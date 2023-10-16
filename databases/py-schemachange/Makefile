PORTNAME=	schemachange
PORTVERSION=	3.6.0
CATEGORIES=	databases python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	A Database Change Management tool for Snowflake
WWW=		https://github.com/Snowflake-Labs/schemachange

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS=	${PYTHONPREFIX_SITELIBDIR}/setuptools/__init__.py:devel/py-setuptools@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/wheel/__init__.py:devel/py-wheel@${PY_FLAVOR}

WHEEL_DEPENDS=	${PYTHONPREFIX_SITELIBDIR}/jinja2/__init__.py:devel/py-Jinja2@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/pandas/__init__.py:math/py-pandas@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/snowflake/connector/__init__.py:databases/py-snowflake-connector@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/yaml/__init__.py:devel/py-yaml@${PY_FLAVOR}

.include <bsd.port.mk>

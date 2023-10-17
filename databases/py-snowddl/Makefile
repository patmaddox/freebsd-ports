PORTNAME=	snowddl
PORTVERSION=	0.20.0
CATEGORIES=	databases python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	SnowDDL is a declarative-style tool for object management automation in Snowflake.
WWW=		https://docs.snowddl.com/

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent pep517

PY_DEPENDS=	${PYTHON_PKGNAMEPREFIX}jsonschema>=4.18:devel/py-jsonschema@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pydantic2>=2.4:devel/py-pydantic2@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}yaml>=6.0:devel/py-yaml@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}snowflake-connector>=3.0:databases/py-snowflake-connector@${PY_FLAVOR}

BUILD_DEPENDS=	wheel-${PYTHON_VER}:devel/py-wheel@${PY_FLAVOR} \
		${PY_DEPENDS}

RUN_DEPENDS=	${PY_DEPENDS}

.include <bsd.port.mk>

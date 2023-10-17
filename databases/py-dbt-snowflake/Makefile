PORTNAME=	dbt-snowflake
PORTVERSION=	1.6.0
CATEGORIES=	databases python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	dbt adapter for Snowflake
WWW=		https://github.com/dbt-labs/dbt-snowflake

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	concurrent distutils

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}agate>0:textproc/py-agate@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}dbt-core>0:databases/py-dbt-core@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}snowflake-connector>0:databases/py-snowflake-connector@${PY_FLAVOR}

.include <bsd.port.mk>

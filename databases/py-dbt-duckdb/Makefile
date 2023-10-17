PORTNAME=	dbt-duckdb
PORTVERSION=	1.6.0
CATEGORIES=	databases python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	dbt adapter for DuckDB
WWW=		https://github.com/jwills/dbt-duckdb

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent distutils

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}dbt-core>0:databases/py-dbt-core@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}duckdb>0:databases/py-duckdb@${PY_FLAVOR}

.include <bsd.port.mk>

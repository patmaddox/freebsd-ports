PORTNAME=	dbt-core
PORTVERSION=	1.6.0
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	dbt enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
WWW=		https://github.com/dbt-labs/dbt-core

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent distutils

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}agate>0:textproc/py-agate@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}Jinja2>0:devel/py-Jinja2@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}mashumaro>0:devel/py-mashumaro@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}logbook>0:devel/py-logbook@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}click>0:devel/py-click@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}networkx>0:math/py-networkx@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}colorama>0:devel/py-colorama@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pathspec>0:devel/py-pathspec@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}isodate>0:devel/py-isodate@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}sqlparse>0:databases/py-sqlparse@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}dbt_extractor>0:databases/py-dbt_extractor@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}hologram>0:devel/py-hologram@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}minimal-snowplow-tracker>0:devel/py-minimal-snowplow-tracker@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}dbt-semantic-interfaces>0:devel/py-dbt-semantic-interfaces@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}packaging>0:devel/py-packaging@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}protobuf>0:devel/py-protobuf@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pytz>0:devel/py-pytz@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}yaml>0:devel/py-yaml@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}typing-extensions>0:devel/py-typing-extensions@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}cffi>0:devel/py-cffi@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}idna>0:dns/py-idna@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}requests>0:www/py-requests@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}urllib3>0:net/py-urllib3@${PY_FLAVOR}

.include <bsd.port.mk>

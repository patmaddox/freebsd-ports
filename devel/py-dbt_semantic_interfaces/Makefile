PORTNAME=	dbt_semantic_interfaces
PORTVERSION=	0.2.0
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	The shared semantic layer definitions that dbt-core and MetricFlow use.
WWW=		https://github.com/dbt-labs/dbt-semantic-interfaces

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS+= hatch:devel/py-hatch@${PY_FLAVOR} \
		hatchling:devel/py-hatchling@${PY_FLAVOR}

#RUN_DEPENDS+= 	${PYTHONPREFIX_SITELIBDIR}/agate:textproc/py-agate@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/colorama:devel/py-colorama@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/click:devel/py-click@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/dateutil:devel/py-dateutil@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/google/protobuf:devel/py-protobuf@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/hologram:devel/py-hologram@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/jinja2:devel/py-Jinja2@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/jsonschema:devel/py-jsonschema@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/logbook:devel/py-logbook@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/mashumaro:devel/py-mashumaro@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/msgpack:devel/py-msgpack@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pathspec:devel/py-pathspec@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pytz:devel/py-pytz@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/requests:www/py-requests@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/snowplow_tracker:devel/py-minimal-snowplow-tracker@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/typing_extensions.py:devel/py-typing-extensions@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/yaml:devel/py-yaml@${PY_FLAVOR}

#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}
#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}

.include <bsd.port.mk>

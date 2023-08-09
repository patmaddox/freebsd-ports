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

RUN_DEPENDS= 	${PYTHONPREFIX_SITELIBDIR}/agate/__init__.py:textproc/py-agate@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/colorama/__init__.py:devel/py-colorama@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/click/__init__.py:devel/py-click@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/dateutil/__init__.py:devel/py-dateutil@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/dbt_extractor/__init__.py:devel/py-dbt_extractor@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/dbt_semantic_interfaces/__init__.py:devel/py-dbt_semantic_interfaces@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/google/protobuf/__init__.py:devel/py-protobuf@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/hologram/__init__.py:devel/py-hologram@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/jinja2/__init__.py:devel/py-Jinja2@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/jsonschema/__init__.py:devel/py-jsonschema@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/logbook/__init__.py:devel/py-logbook@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/mashumaro/__init__.py:devel/py-mashumaro@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/more_itertools/__init__.py:devel/py-more-itertools@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/msgpack/__init__.py:devel/py-msgpack@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/networkx/__init__.py:math/py-networkx@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/pathspec/__init__.py:devel/py-pathspec@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/pydantic/__init__.py:devel/py-pydantic@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/pytz/__init__.py:devel/py-pytz@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/requests/__init__.py:www/py-requests@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/snowplow_tracker/__init__.py:devel/py-minimal-snowplow-tracker@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/sqlparse/__init__.py:databases/py-sqlparse@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/typing_extensions.py:devel/py-typing-extensions@${PY_FLAVOR} \
	${PYTHONPREFIX_SITELIBDIR}/yaml/__init__.py:devel/py-yaml@${PY_FLAVOR}

.include <bsd.port.mk>

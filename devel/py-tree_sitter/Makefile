PORTNAME=	tree_sitter
PORTVERSION=	0.20.1
CATEGORIES=	devel python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
MASTER_SITES=	PYPI
MAINTAINER=	pat@patmaddox.com
COMMENT=	Python bindings to the Tree-sitter parsing library
WWW=		https://github.com/tree-sitter/py-tree-sitter

LICENSE=	MIT

USES=		python
USE_PYTHON=	autoplist concurrent distutils

LIB_DEPENDS=	libtree-sitter.so:devel/tree-sitter

#BUILD_DEPENDS=	maturin:devel/py-maturin@${PY_FLAVOR}

#RUN_DEPENDS+= 	${PYTHONPREFIX_SITELIBDIR}/agate:textproc/py-agate@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/colorama:devel/py-colorama@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/click:devel/py-click@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/dateutil:devel/py-dateutil@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/dbt_semantic_interfaces:devel/py-dbt_semantic_interfaces@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/google/protobuf:devel/py-protobuf@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/hologram:devel/py-hologram@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/jinja2:devel/py-Jinja2@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/jsonschema:devel/py-jsonschema@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/logbook:devel/py-logbook@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/mashumaro:devel/py-mashumaro@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/msgpack:devel/py-msgpack@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/networkx:math/py-networkx@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pathspec:devel/py-pathspec@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pydantic:devel/py-pydantic@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pytz:devel/py-pytz@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/requests:www/py-requests@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/snowplow_tracker:devel/py-minimal-snowplow-tracker@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/typing_extensions.py:devel/py-typing-extensions@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/yaml:devel/py-yaml@${PY_FLAVOR}

#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}
#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}

.include <bsd.port.mk>

PORTNAME=	dbt_extractor
PORTVERSION=	0.4.1
CATEGORIES=	devel python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
MASTER_SITES=	PYPI
MAINTAINER=	pat@patmaddox.com
COMMENT=	A tool that processes the most common jinja value templates in dbt model files
WWW=		https://github.com/dbt-labs/dbt-parser-generator/
DISTFILES=	${PORTNAME}-${PORTVERSION}.tar.gz

LICENSE=	APACHE20

USES=		cargo python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS=	maturin:devel/py-maturin@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/tree_sitter/__init__.py:devel/py-tree_sitter@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/tree_sitter_jinja2/__init__.py:devel/tree-sitter-jinja2

RUN_DEPENDS=	${PYTHONPREFIX_SITELIBDIR}/tree_sitter/__init__.py:devel/py-tree_sitter \
		${PYTHONPREFIX_SITELIBDIR}/tree_sitter_jinja2/__init__.py:devel/tree-sitter-jinja2

CARGO_BUILD=	no
CARGO_INSTALL=	no

pre-build:
	cd ${WRKDIR}/${PORTNAME}-${PORTVERSION} && maturin build -f
	mkdir ${WRKDIR}/${PORTNAME}-${PORTVERSION}/dist
	cp ${WRKDIR}/${PORTNAME}-${PORTVERSION}/target/wheels/${PORTNAME}-*freebsd*.whl ${WRKDIR}/${PORTNAME}-${PORTVERSION}/dist/

post-extract:
	ln -s ${WRKDIR}/tree-sitter-jinja2-*/ ${WRKDIR}/${PORTNAME}-${PORTVERSION}/tree-sitter-dbt-jinja

.include <bsd.port.mk>

PORTNAME=	dbt_extractor
PORTVERSION=	0.4.1
CATEGORIES=	devel python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
MASTER_SITES=	PYPI
MAINTAINER=	pat@patmaddox.com
COMMENT=	A tool that processes the most common jinja value templates in dbt model files
WWW=		https://github.com/dbt-labs/dbt-extractor/
DISTFILES=	${PORTNAME}-${PORTVERSION}.tar.gz

LICENSE=	APACHE20

USES=		cargo python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS=	maturin:devel/py-maturin@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}tree_sitter>0:devel/py-tree_sitter@${PY_FLAVOR}

CARGO_BUILD=	no
CARGO_INSTALL=	no

pre-build:
	cd ${WRKDIR}/${PORTNAME}-${PORTVERSION} && maturin build -f
	mkdir ${WRKDIR}/${PORTNAME}-${PORTVERSION}/dist
	cp ${WRKDIR}/${PORTNAME}-${PORTVERSION}/target/wheels/${PORTNAME}-*freebsd*.whl ${WRKDIR}/${PORTNAME}-${PORTVERSION}/dist/

post-extract:
	ln -s ${WRKDIR}/tree-sitter-jinja2-*/ ${WRKDIR}/${PORTNAME}-${PORTVERSION}/tree-sitter-dbt-jinja

do-test:
	@(cd ${TEST_WRKSRC} && ${SETENV} ${TEST_ENV} PYO3_PYTHON=${PYTHON_CMD} ${CARGO} test)


.include <bsd.port.mk>

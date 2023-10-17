PORTNAME=	dbt-extractor
PORTVERSION=	0.4.1
CATEGORIES=	devel python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
MASTER_SITES=	PYPI
MAINTAINER=	pat@patmaddox.com
COMMENT=	A tool that processes the most common jinja value templates in dbt model files
WWW=		https://github.com/dbt-labs/dbt-extractor/
DISTNAME=	dbt_extractor-${PORTVERSION}
DISTFILES=	${DISTNAME}.tar.gz

LICENSE=	APACHE20

USES=		cargo python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS=	maturin:devel/py-maturin@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}tree-sitter>0:devel/py-tree-sitter@${PY_FLAVOR}

CARGO_BUILD=	no
CARGO_INSTALL=	no

post-extract:
	ln -s ${WRKDIR}/tree-sitter-jinja2-*/ ${WRKSRC}/tree-sitter-dbt-jinja

pre-build:
	cd ${WRKSRC} && maturin build -f
	mkdir ${WRKSRC}/dist
	cp ${WRKSRC}/target/wheels/${DISTNAME}-*freebsd*.whl ${WRKSRC}/dist/

do-test:
	@(cd ${TEST_WRKSRC} && ${SETENV} ${TEST_ENV} PYO3_PYTHON=${PYTHON_CMD} ${CARGO} test)


.include <bsd.port.mk>

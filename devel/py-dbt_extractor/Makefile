PORTNAME=	dbt_extractor
PORTVERSION=	0.5.0
CATEGORIES=	devel python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
USE_GITHUB=	yes
#USE_GITHUB=	nodefault
#MASTER_SITES=	https://files.pythonhosted.org/packages/9b/51/50458dc1e1fa985a46ebb350cb61d4fc0d0f3fe00ae55c7e614f25801865/
#MASTER_SITES=	PYPI
MAINTAINER=	pat@patmaddox.com
COMMENT=	A tool that processes the most common jinja value templates in dbt model files
WWW=		https://github.com/dbt-labs/dbt-parser-generator/
DISTFILES=	dbt-extractor-${PORTVERSION}.tar.gz # dbt_extractor-${PORTVERSION}-cp38-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl

LICENSE=	APACHE20

GH_ACCOUNT=	dbt-labs
GH_PROJECT=	dbt-extractor
GH_TAGNAME=	83f0d93d4d5537de3960ac5659f72f430f5d7d5d

USES=		cargo python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS=	maturin:devel/py-maturin@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/tree_sitter:devel/py-tree_sitter@${PY_FLAVOR}
#		pip:devel/py-pip@${PY_FLAVOR}

RUN_DEPENDS=	${PYTHONPREFIX_SITELIBDIR}/tree_sitter:devel/py-tree_sitter@${PY_FLAVOR}

CARGO_BUILD=	no
CARGO_INSTALL=	no

#PLIST_FILES=	lib/libdbt_extractor.so

pre-build:
	cd ${WRKDIR}/dbt-extractor-${GH_TAGNAME} && maturin build -f
	mkdir ${WRKDIR}/dbt-extractor-${GH_TAGNAME}/dist
	cp ${WRKDIR}/dbt-extractor-${GH_TAGNAME}/target/wheels/dbt_extractor-*freebsd*.whl ${WRKDIR}/dbt-extractor-${GH_TAGNAME}/dist/

post-extract:
	ln -s ${WRKDIR}/tree-sitter-jinja2-0.2.0 ${WRKDIR}/dbt-extractor-${GH_TAGNAME}/tree-sitter-dbt-jinja

#post-install:	
#	${INSTALL_LIB} ${WRKDIR}/dbt-extractor-${GH_TAGNAME}/target/release/libdbt_extractor.so ${STAGEDIR}${PREFIX}/lib

.include <bsd.port.mk>

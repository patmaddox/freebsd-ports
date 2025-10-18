PORTNAME=	emacs-libvterm
DISTVERSION=	20250929.1514
CATEGORIES=	comms

MAINTAINER=	pat@patmaddox.com
COMMENT=	Emacs libvterm integration
WWW=		https://github.com/akermu/emacs-libvterm

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/LICENSE

LIB_DEPENDS=	libvterm.so:devel/libvterm

USES=		emacs:build cmake:noninja
USE_GITHUB=	yes
GH_ACCOUNT=	akermu
GH_TAGNAME=	adf8d10212d15f9bd5ca62b96c7b423be02ce3c4

do-configure:
	${MKDIR} ${WRKSRC}/build
	cd ${WRKSRC}/build && ${CMAKE_BIN} ${CMAKE_ARGS} ..

do-build:
	cd ${WRKSRC}/build && ${MAKE}

do-install:
	${INSTALL_DATA} ${WRKSRC}/vterm.el ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}
	${INSTALL_LIB} ${WRKSRC}/vterm-module.so ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}

.include <bsd.port.mk>

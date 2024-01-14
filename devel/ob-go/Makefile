PORTNAME=	ob-go
PORTVERSION=	20190201.2040
CATEGORIES=	devel

MAINTAINER=	pat@patmaddox.com
COMMENT=	Org-Babel support for evaluating go code
WWW=		https://github.com/pope/ob-go

LICENSE=	GPLv3+

RUN_DEPENDS=	${PREFIX}/${EMACS_SITE_LISPDIR}/go-mode.el:devel/go-mode.el

USES=			emacs go
EMACS_NO_DEPENDS=	yes

USE_GITHUB=	yes
GH_ACCOUNT=	pope
GH_PROJECT=	ob-go
GH_TAGNAME=	2067ed5

NO_ARCH=	yes
NO_BUILD=	yes

do-install:
	@${MKDIR} ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}
	${INSTALL_DATA} ${WRKSRC}/ob-go.el ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}

.include <bsd.port.mk>

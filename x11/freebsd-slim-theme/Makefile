# New ports collection makefile for: slim in live mode
# Date created:        11 may 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	freebsd-slim-theme
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD theme for slim and autologin too

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

RUN_DEPENDS=	slim:x11/slim \

NO_BUILD=	yes

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/slim/themes/freebsd
	${CP} -R ${WRKSRC}/fbsd/* ${STAGEDIR}/${PREFIX}/share/slim/themes/freebsd/
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd/slim/etc
	${CP} -R ${WRKSRC}/etc/* ${STAGEDIR}/${PREFIX}/share/freebsd/slim/etc/
.include <bsd.port.mk>

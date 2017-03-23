# New ports collection makefile for: mate settings in installed mode
# Date created:        14 jun 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	mate-installed-settings
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD mate settings in installed mode

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

RUN_DEPENDS=	pkg:archivers/pkg

NO_BUILD=	yes

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd/mate-installed-settings
	${CP} -R   ${WRKSRC}/freebsd/* ${STAGEDIR}/${PREFIX}/share/freebsd/mate-installed-settings
.include <bsd.port.mk>

# New ports collection makefile for: kde settings in installed mode
# Date created:        4 Jan 2016
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	kde-installed-settings
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD KDE settings in installed mode

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

RUN_DEPENDS=	pkg:archivers/pkg

NO_BUILD=	yes

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd/kde-settings/etc
	${CP} -Rf   ${WRKSRC}/etc ${STAGEDIR}/${PREFIX}/share/freebsd/kde-settings
.include <bsd.port.mk>

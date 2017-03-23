# New ports collection makefile for: freebsd common settings in live mode
# Date created:        5 july 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	freebsd-live-common-settings
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD common settings in live mode

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves


NO_BUILD=	yes

RUN_DEPENDS= pkg:archivers/pkg \
		sudo:security/sudo

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd
	${CP} -R   ${WRKSRC}/freebsd/* ${STAGEDIR}/${PREFIX}/share/freebsd
	${MKDIR} ${STAGEDIR}/${PREFIX}/etc/polkit-1
	${CP} -R   ${WRKSRC}/etc/polkit-1/* ${STAGEDIR}/${PREFIX}/etc/polkit-1
.include <bsd.port.mk>

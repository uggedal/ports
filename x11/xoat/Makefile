# $OpenBSD$

COMMENT =	obstinate asymetric tiling window manager

VERSION =	20150328
DISTNAME =	${GH_PROJECT}-${VERSION}
CATEGORIES =	x11

MAINTAINER =	Eivind Uggedal <eivind@uggedal.com>

# MIT/X11
PERMIT_PACKAGE_CDROM =	Yes

WANTLIB +=	X11 Xau Xdmcp Xext Xft Xinerama Xrender c expat fontconfig
WANTLIB +=	freetype pthread-stubs xcb z

GH_ACCOUNT =	seanpringle
GH_PROJECT =	xoat
GH_COMMIT =	7ae527002bee2905096487ddf74386e0159051b2

NO_TEST =	Yes

CFLAGS +=	-std=c99

do-install:
	cd ${WRKSRC}; \
	    ${INSTALL_MAN} xoat.1 ${PREFIX}/man/man1/; \
	    ${INSTALL_PROGRAM} xoat ${PREFIX}/bin

.include <bsd.port.mk>

               Code Page Recoder for DOS & OS/2
              ==================================

  This program serves to translate text files encoded in one codepage
for display or use under another codepage.  The currently supported
codepages are:

        437     United States PC
        819     ISO-8859/1 (UNIX)
        850     Multilingual
        860     Portuguese
        863     French-Canadian
        865     Nordic

  The command-line syntax is as follows:

        RECODE [FROM=codepage] [TO=codepage] source > destination

  The source and destination codepages are optional and default to 819
and 850 respectively.  The result is sent to the standard output and
may be redirected to any file but the original source file.

  One side effect of this program with UNIX files is to convert the files
to use cr-lf pairs at the end of text lines instead of the simple linefeeds
that mark the end of UNIX text file lines.  This results in an output
file larger than the source file.

  The source code and make file (MSC 6.00a) are included.  The information
required to make this program were obtained from an IBM reference document
packaged with OS/2 1.2, from an Internet FAQ sheet about the ISO-8859-1
character set standard, and from one of the help topics in the IBM
Presentation Manager Guide & Reference, packaged with the IBM OS/2
Developer's Toolkit.

  Questions, suggestions, criticisms to:

        Rick Papo
        Internet: rpapo@msen.com
        CompuServe: 72607,3111


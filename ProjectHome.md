ASN1Parser is ASN.1(Abstract Syntax Notation 1) parser for 3GPP specifications (specially RRC, S1AP, X2AP).

ASN1Parserは3GPP標準に記載されたASN.1(抽象構文記法.1)を解読するための構文解析器です。
特にRRC(TS36.331)、S1AP(TS36.413)、X2AP(TS36.423)プロトコルを対象としています。

ASN1ParserはC#(CSharp)で記述しています。

構文解析部分はLALR(1)パーサジェネレータである『caper』を利用させていただいております。
(caper - http://caper.googlecode.com/svn/trunk/caper/site/caper.html)
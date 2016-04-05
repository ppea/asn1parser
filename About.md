#About ASN1Parser

# ASN1Parserについて #

ASN1Parserは3GPP標準を読み解くにあたり、
そこに記載されたASN.1の理解を手助けするために作成した、
いわゆる「なんちゃって」ASN.1パーサです。

ASN1Parserの目的はあくまでASN.1の読解であり、
バイナリエンコード／デコードは目的としていませんのでご了承ください。

# ASN1Parserの目的 #

ASN1Parserが対象としているのは、
3GPP Release8およびRelease9で規定されたLTE(Long Term Evolution)の
RRC(TS36.331)、S1AP(TS36.413)、X2AP(TS36.423)プロトコル中に記載されたASN.1です。

現状、実装上の問題により、ASN.1の最も基本的な
  * 型割当て(Type Assignment)
  * 値割当て(Value Assignment)
以外の構文を使用したASN.1の解析ができません。

よって、たとえば
  * オブジェクト割当て
  * オブジェクトクラス割当て
  * パラメータ化
を使ったASN.1の解析はできません。

S1AP、X2APプロトコルは後者のASN.1構文を好んで(?)使っていますが、
ASN1Parserではこれを汎用性のない方法で処理してしまっています。
================================================================================
MICROSOFT FOUNDATION CLASS ライブラリ: HotelPMS プロジェクトの概要
===============================================================================

アプリケーション ウィザードが作成した HotelPMS には Microsoft 
Foundation Class の基本的な使い方が示されています。アプリケーション作成のひな型
としてお使いください。

このファイルには HotelPMS アプリケーションを構成している各ファイ
ルの概要説明が含まれます。

HotelPMS.vcproj
   これはアプリケーション ウィザードで生成された VC++ プロジェクトのメイン プ
   ロジェクト ファイルです。ファイルが生成された Visual C++ のバージョン情報が
   含まれています。また、アプリケーション ウィザードで選択したプラットフォー
   ム、構成およびプロジェクト機能に関する情報も含まれています。

HotelPMS.h
   これはアプリケーションのメイン ヘッダー ファイルです。このファイルには、
   Resource.h を含む、その他のプロジェクト固有のヘッダーが含まれていて、
   CHotelPMSApp アプリケーション クラスを宣言します。

HotelPMS.cpp
   これは、アプリケーション クラス CHotelPMSApp を含むメイン アプリケー
   ション ソース ファイルです。

HotelPMS.rc
   これは、プログラムが使用する Microsoft Windows のリソースの一覧ファイルで
   す。このファイルには RES サブディレクトリに保存されているアイコン、ビットマ
   ップ、カーソルが含まれています。このファイルは、Microsoft Visual C++ で直接
   編集することができます。プロジェクト リソースは 1041 にあります。

res\HotelPMS.ico
   これは、アプリケーションのアイコンとして使用されるアイコンファイルです。この
   アイコンはメイン リソース ファイル HotelPMS.rc に含まれていま
   す。

res\HotelPMS.rc2
   このファイルは Microsoft Visual C++ を使用しないで編集されたリソースを含んで
   います。リソース エディタで編集できないリソースはすべてこのファイルに入れて
   ください。
HotelPMS.reg
   このレジストリ ファイルは、フレームワークの登録設定方法を紹介するためのサン
   プルファイルです。
   アプリケーションと一緒に .reg ファイルとして使用するか、または削除して既定
   の登録 RegisterShellFileTypes を使用します。


/////////////////////////////////////////////////////////////////////////////

メイン フレーム ウィンドウ:
    プロジェクトは標準の MFC インターフェイスを含みます。

MainFrm.h, MainFrm.cpp
   これらのファイルは、フレーム クラス CMainFrame を含みます。
   フレーム クラスは CMDIFrameWnd から派生し、すべての MDI フレーム機能を制御
   します。

res\Toolbar.bmp
   このビットマップ ファイルはツール バーのタイル イメージとして使用されます。
   初期ツール バーおよびステータス バーは、CMainFrame クラスで
   作成されます。ツール バーのボタンを追加するには、このツール バーのビットマッ
   プをリソース エディタを使用して編集し、HotelPMS.rc ファイル内
   の IDR_MAINFRAME TOOLBAR 配列を更新してください。
/////////////////////////////////////////////////////////////////////////////

子フレーム ウィンドウ:

ChildFrm.h, ChildFrm.cpp
   これらのファイルは、MDI アプリケーションの子ウィンドウをサポートする 
   CChildFrame クラスの定義と実装を行います。

/////////////////////////////////////////////////////////////////////////////

アプリケーション ウィザードは 1 つのドキュメントの種類と 1 つのビューを作成し
ます:

HotelPMSDoc.h, HotelPMSDoc.cpp - ドキュメント
   これらのファイルは CHotelPMSDoc クラスを含みます。特別なドキュメント 
   データを追加したり、ファイルを保存したり、
   (via CHotelPMSDoc::Serialize) を読み込んだりするには、これらのファイ
   ルを編集してください。
    ドキュメントには次の文字列が含まれます:
        ファイルの拡張子:             pms
        ファイルの種類のID:           HotelPMS.Document
        メイン フレーム キャプション: HotelPMS
        ドキュメントの種類の名前:     HotelPMS
        フィルタ名:                   HotelPMS Files (*.pms)
        ファイルの新しい短い名前:     HotelPMS
        ファイルの種類の長い名前:     HotelPMS.Document

HotelPMSView.h, HotelPMSView.cpp - ドキュメントのビュー
   これらのファイルは CHotelPMSView クラスを含みます。
   CHotelPMSView オブジェクトは CHotelPMSDoc オブジェクトを表示す
   るのに使用されます。

res\HotelPMSDoc.ico
   このファイルは、CHotelPMSDoc クラスの MDI 子ウィンドウ用アイコンとし
   て使用されるアイコン ファイルです。このアイコンは、メイン リソースファイル 
   HotelPMS.rc に含まれています。


/////////////////////////////////////////////////////////////////////////////

その他の機能:

ActiveX コントロール
   アプリケーションは ActiveX コントロールの使用に関するサポートを含みます。

印刷と印刷プレビューのサポート
   アプリケーション ウィザードは、 MFC ライブラリから CView クラスのメンバ関数
   を呼び出すことによって、印刷、印刷の設定、および印刷プレビュー コマンドを処
   理するコードを生成しました。

データベース サポート
   アプリケーション ウィザードは、プログラムに基本レベルのデータベース サポート
   を追加しました。必要なファイルのみ含まれています。

Windows ソケット
   アプリケーションは TCP/IP ネットワーク経由の通信を確立するためのサポートを
   含みます。

/////////////////////////////////////////////////////////////////////////////

その他の標準ファイル:

StdAfx.h, StdAfx.cpp
   これらのファイルは、既にコンパイルされたヘッダー ファイル (PCH) 
   HotelPMS.pch や既にコンパイルされた型のファイル StdAfx.obj を
   ビルドするために使用されます。

Resource.h
   これは新規リソース ID を定義する標準ヘッダー ファイルです。Microsoft 
   Visual C++ はこのファイルの読み取りと更新を行います。

HotelPMS.manifest
   アプリケーション マニフェスト ファイルは Windows XP で、Side-by-Side アセン
   ブリの特定のバージョンに関するアプリケーションの依存関係を説明するために使用
   されます。ローダーはこの情報を使用して、アセンブリ キャッシュから適切なアセ
   ンブリを、またはアプリケーションからプライベート アセンブリを読み込みます。
   アプリケーション マニフェストは再頒布用に、実行可能アプリケーションと同じフ
   ォルダにインストールされる外部 .manifest ファイルとして含まれているか、また
   はリソースのフォーム内の実行可能ファイルに含まれています。
/////////////////////////////////////////////////////////////////////////////

その他の注意:

アプリケーション ウィザードは "TODO:" で始まるコメントを使用して、追加したりカ
スタマイズする必要があるソース コードの部分を示します。

アプリケーションが共有 DLL 内で MFC を使用する場合は、MFC DLL を再頒布する必要
があります。また、アプリケーションがオペレーティング システムのロケール以外の言
語を使用している場合も、対応するローカライズされたリソース MFC80XXX.DLL を再頒
布する必要があります。これらのトピックの詳細については、MSDN ドキュメントの 
Visual C++ アプリケーションの再頒布に関するセクションを参照してください。

/////////////////////////////////////////////////////////////////////////////

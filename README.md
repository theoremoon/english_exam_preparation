# english_exam_preparation
 これは、私の英語の試験対策用あれです。Python3.xで動くはずです

# options
 -f <file>で、指定したファイル名のファイルを問題ファイルとして開きます。問題ファイルのフォーマットは後述します。

 -l <level>で、指定したレベルで問題を出題します。レベルに応じて、虫食いの個数が増えます。指定がない場合は、ランダムでレベルを決定しますが、多くの場合にすべて虫食いとなります。

# problem file format
 問題ファイルのフォーマットを示します。問題ファイルの文字コードはutf-8としています。問題ファイルは、「英文」「和文」「空行」の３つから構成されます。このプログラムは問題ファイルの最初の行を「英文」、それに続く行を「和文」、次を「空行」と認識します。途中に改行のある文は許されません。また、この仕様のため、問題ファイルの最後には空行が必ず必要です。

 和文を構成する要素に指定はありませんが、英文には英語の多様性に対応するための構文を用意しています。例えば、"I don't like him."と、"I do not like him."は同じ意味ですが違うものと解釈されるでしょう。そこで、"I (don't|do not) like him."と記述することで、don'tまたはdo notと認識されるように指定できます。これを利用して、(that|)などと書けばthatを入れても入れなくても良い、というしていにできます。ただし、これらの指定を行った場合、表示される虫食いの穴の数と、単語の大きさ　数が合わなくなります。

# change log
 かかないです。

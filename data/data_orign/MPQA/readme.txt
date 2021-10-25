【MPQA-dataset】

docs：每个子文件夹中为一个文档，文件夹名为文档的parent

meta_anns：文档的信息，如来源、日期等

以下文件无meta_anns : 20020516/22.23.24-9583, 
    20020517/22.08.22-24562, 20020521/22.21.24-5526, 
    20020522/22.34.49-13286, and 20020523/22.37.46-10374.

gate_anns：GATE标注好的文件，xml格式
具体标注含义

man_anns：手动标注的文件，共有2类名字：
1、gateman.mpqa.lre.3.0： 标注意义同gate，具体格式为：id\t起点，终点\t标注内容
形如：5	716,725	attitude	intensity="low" id="a5" attitude-type="intention-pos" targetFrame-link="tfa5" 
2、gatesentences.mpqa.2.0： 手工删去了无关垃圾语句，保留gate语句
形如：12	709,1028	string	GATE_sentence

target：已标注起止点
sentiment：有polarity、attitude-type等情绪专有属性
document：所有文件都在docs文件夹，在每个大目录中对应的文件夹/文件名是一样的



【MitchellEtal】
语料都在10-fold里，有train，test各10个。其中一条tweet按空格切分，然后再一一标注。
如：
## Tweet 1941
Lindsey	B-PERSON	positive
,	O	_
I	O	_
look	O	_
forward	O	_
to	O	_
your	O	_
October	B-DATE	_
17	I-DATE	_
show	O	_
in	O	_
Anaheim	B-PLACE	_
!	O	_
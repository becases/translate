# translate

usage: trans.exe [-h] [-f F] [-t T] [-q Q]

-h   help

-f    原文语种，不确定可设置为auto

-t    目标语种

-q   需要翻译的词

如不输入-f则-f默认值为auto，如不输入-t则-f默认值为zh，如不输入-q则默认值为空格

语种列表

源语言语种不确定时可设置为 auto，目标语言语种不可设置为 auto。但对于非常用语种，语种自动检测可能存在误差。

自动检测    auto

中文    zh

英语    en

粤语    yue

文言文  wyw

日语    jp

韩语    kor

法语    fra

西班牙语spa

泰语    th

阿拉伯语ara

俄语    ru

葡萄牙语pt

德语    de

意大利语it

希腊语  el

荷兰语  nl

波兰语  pl

保加利亚语bul

爱沙尼亚语est

丹麦语  dan

芬兰语  fin

捷克语  cs

罗马尼亚语rom

斯洛文尼亚语slo

瑞典语  swe

匈牙利语hu

繁体中文cht

越南语  vie

如何在一次请求中翻译多个单词或者多段文本?

您可以在发送的字段q中用换行符（在多数编程语言中为转义符号 \n。其中\n是需要能被程序解析出来的换行符而不是字符串\n，您可以将\n用引号包围 ）或者回车换行来分隔要翻译的多个单词或者多段文本，这样您就能得到多段文本独立的翻译结果了。

单次翻译请求是否有字符数限制？

请将单次翻译文本长度限定为6000字节以内（汉字约为2000个字符）。此外，高频单次请求文本过长或将导致翻译超时。您可将q值分多次请求。

为什么我的请求会返回54003？

54003表示调用频率超限，请降低调用频率。您的QPS（每秒请求量）=1

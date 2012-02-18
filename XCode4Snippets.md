善用XCode 4的Snippets功能进行代码补全

XCode 4提供了Snippets的功能，你可以自定义自己的Snippets，从而减少编程中的重复性输入工作。
在Xcode 4右侧的工具区域的资源库这边你可以找到代码片段库，你可以看到XCode已经自带的一些Snippets:

![代码片段](img/xcode_snippet.png?raw=true)

比如你需要写一个dealloc方法，你只需要输入

	dealloc
	
然后根据建议回车，便可以得到如下结果，你需要输入自己创建的变量的释放工作了。

![dealloc](img/dealloc.png?raw=true)

当我们需要自己的Snippet时，你可以将代码片段拖进Snippets区域，这个时候会新建一个Snippet，你需要对其进行编辑，编辑标题，描述以及最重要的Completion shortcut，比如你想创建一个自动完成属性声明的代码。

	@property (nonatomic, retain) <#type#> *<#name#>;

将上面的代码拷进XCode，然后拖进Snippet，编辑Completion shortcut为rrr，
那么下次你输入rrr的时候，XCode便会提示你输入如上的代码片段。
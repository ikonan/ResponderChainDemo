# ResponderChainDemo
一种基于ResponderChain的对象交互方式(代码demo)

传统iOS的对象间交互模式就那么几种：直接property传值、delegate、KVO、block、protocol、多态、Target-Action。但是有一天我在跟同事小龙结对编程的时候，他向我介绍了一个全新的交互方式：基于ResponderChain来实现对象间交互。

这种方式通过在UIResponder上挂一个category，使得事件和参数可以沿着responder chain逐步传递。

这相当于借用responder chain实现了一个自己的事件传递链。这在事件需要层层传递的时候特别好用，然而这种对象交互方式的有效场景仅限于在responder chain上的UIResponder对象上。

详细文章请参见：https://casatwy.com/responder_chain_communication.html

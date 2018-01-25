aio_windows_patch
===============================

* version: 0.0.1
* status: dev
* author: hsz
* email: hsz1273327@gmail.com

Desc
--------------------------------

到目前为止Python的asyncio版本对windows的支持都非常差,尤其是`loop.add_signal_handler`在windows
下无法处理signal模块下的信号.

``https://codereview.appspot.com/119990043/``  上有一个补丁修复了这一问题.只是不知道为什么一直
没有被官方使用,这个项目就是将这个补丁提取出来做成的.

这个问题怎么也会被官方解决的,当解决了这个项目就可以删掉了.


keywords:asyncio,patch


Feature
----------------------

* loop.add_signal_handler 可以在windows下处理信号

Example
-------------------------------

.. code:: python

    import aio_windows_patch as asyncio

    ....

Install
--------------------------------

- ``python -m pip install aio_windows_patch``

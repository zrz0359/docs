
.. _cn_api_paddle_cauchy_:

cauchy_
-------------------------------
   .. py:function:: paddle.cauchy_(x: paddle.Tensor, loc: Numeric = 0, scale: Numeric = 1, name: str | None = None)→ paddle.Tensor[source]

.. note::
    paddle.Tensor请参见 `source`_ .

        .. _Tensor 介绍: ../../guides/beginner/paddle.Tensor_cn.html#id7

参数
:::::::::
x (Tensor)：填充张量，数据类型为float32或float64。

loc（标量，可选）：分布峰值的位置。数据类型为float32或float64。

scale（标量，可选）：半最大时的半宽度（HWHM）。数据类型为float32或float64。必须是正值。

name（str|无，可选）：详细信息请参考：ref: ‘ api_guide_Name ’。通常，不需要设置。默认值:没有。



返回
:::::::::
张量：从柯西分布中抽取数字的输入张量。



代码示例
:::::::::



Examples:
        .. code-block:: python

            >>> import paddle
            >>> x = paddle.randn([3, 4])
            >>> x.cauchy_(1, 2)
            >>> # doctest: +SKIP('random check')
            >>> print(x)
            Tensor(shape=[3, 4], dtype=float32, place=Place(cpu), stop_gradient=True,
            [[ 3.80087137,  2.25415039,  2.77960515,  7.64125967],
             [ 0.76541221,  2.74023032,  1.99383152, -0.12685823],
             [ 1.45228469,  1.76275957, -4.30458832, 34.74880219]])


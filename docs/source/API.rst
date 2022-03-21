===
API
===

.. py:class:: Astra(namespace: str = 'camera')
.. py:method:: read_rgb()

    :return:
        the cv2 BGR image from the Astra Camera
    :rtype:
        np.ndarray

.. py:method:: read_depth()

    :return:
        a np array of depth from Astra Camera
    :rtype:
        np.ndarray

.. py:method:: get_real_xyz(x, y, depth_img)

    calculates and returns the real xyz coordinates of point (x, y) in depth image

    :param x: the x coordinate of the point
    :type x: int
    :param y: the y coordinate of the point
    :type y: int
    :param depth_img: a depth image, which the return refers to
    :type depth_img: np.ndarray
    :return: a tuple containing (x, y, z)
    :rtype: Tuple[int, int, int]

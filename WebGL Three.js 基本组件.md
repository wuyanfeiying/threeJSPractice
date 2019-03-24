## three.js基本组件
- 场景
- 几何与网格对象
- 相机
---
## 常用组件
- 相机：决定哪些东西将被显示在屏幕上
- 光源：生成阴影与改变物体表面显示效果
- 物体：相机透视图里主要的渲染对象
---
### 场景-基本功能
- scene.add() 在场景中移除物体
- scene.remove() 从场景中移除物体
- scene.getChildByName()获取场景中所有对象的列表
- fog 通过该属性可以设置场景的雾化效果。
- overrideMaterial 通过这个熟悉可以让场景中的所有物体都使用相同材质。
- children 返回所有对象的列表，包括相机和光源对象

### 相机-PerspectiveCamera-透视投影
- fov 视野宽度
- aspect 长宽比，推荐使用 window.innerWidth/window.height
- near 近裁面，推荐值0.1
- far 远裁面，推荐值1000，值太大会影响性能，值太小场景显示不全

### 相机-OrthographicCamera-正射投影
- left 左边界
- right 右边界
- top 上边界
- bottom 下边界
- near 近裁面
- far 远裁面

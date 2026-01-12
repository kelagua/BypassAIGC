## 1.直接改 app.spec（推荐你先试这个）
把你的 excludes=[ ... ] 改成：
```code
excludes=[
    'tkinter',
    'matplotlib',
    'numpy',
    'pandas',
    'scipy',
    'PIL',
    'pkg_resources',   # 关键：避免 pyi_rth_pkgres 运行时 hook
]
```
## 2.修改requirements.txt
```code
# 打包工具
pyinstaller==6.3.0
setuptools<81
```
## 3.修改workflow
```code

```

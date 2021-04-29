# automatic-verilog

---

```verilog
 ▄▄▄▄▄▄▄▄▄▄▄ ▄         ▄ ▄▄▄▄▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄▄▄▄▄ ▄▄       ▄▄ ▄▄▄▄▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄▄▄▄▄ 
▐░░░░░░░░░░░▐░▌       ▐░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░░▌     ▐░░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░░░░░░░░░░░▌
▐░█▀▀▀▀▀▀▀█░▐░▌       ▐░▌▀▀▀▀█░█▀▀▀▀▐░█▀▀▀▀▀▀▀█░▐░▌░▌   ▐░▐░▐░█▀▀▀▀▀▀▀█░▌▀▀▀▀█░█▀▀▀▀ ▀▀▀▀█░█▀▀▀▀▐░█▀▀▀▀▀▀▀▀▀ 
▐░▌       ▐░▐░▌       ▐░▌    ▐░▌    ▐░▌       ▐░▐░▌▐░▌ ▐░▌▐░▐░▌       ▐░▌    ▐░▌         ▐░▌    ▐░▌          
▐░█▄▄▄▄▄▄▄█░▐░▌       ▐░▌    ▐░▌    ▐░▌       ▐░▐░▌ ▐░▐░▌ ▐░▐░█▄▄▄▄▄▄▄█░▌    ▐░▌         ▐░▌    ▐░▌          
▐░░░░░░░░░░░▐░▌       ▐░▌    ▐░▌    ▐░▌       ▐░▐░▌  ▐░▌  ▐░▐░░░░░░░░░░░▌    ▐░▌         ▐░▌    ▐░▌          
▐░█▀▀▀▀▀▀▀█░▐░▌       ▐░▌    ▐░▌    ▐░▌       ▐░▐░▌   ▀   ▐░▐░█▀▀▀▀▀▀▀█░▌    ▐░▌         ▐░▌    ▐░▌          
▐░▌       ▐░▐░▌       ▐░▌    ▐░▌    ▐░▌       ▐░▐░▌       ▐░▐░▌       ▐░▌    ▐░▌         ▐░▌    ▐░▌          
▐░▌       ▐░▐░█▄▄▄▄▄▄▄█░▌    ▐░▌    ▐░█▄▄▄▄▄▄▄█░▐░▌       ▐░▐░▌       ▐░▌    ▐░▌     ▄▄▄▄█░█▄▄▄▄▐░█▄▄▄▄▄▄▄▄▄ 
▐░▌       ▐░▐░░░░░░░░░░░▌    ▐░▌    ▐░░░░░░░░░░░▐░▌       ▐░▐░▌       ▐░▌    ▐░▌    ▐░░░░░░░░░░░▐░░░░░░░░░░░▌
 ▄         ▀ ▀▀▀▀▄▀▄▄▄▄▄▄▄▄▄▄▄▀▄▄▄▄▄▄▄▄▄▄▄▀▄▄▄▄▄▄▄▄▄▄▄ ▄   ▀ ▀     ▄▄▄▄▄▄▄▄▄▄▄▀▄▄▄▄▄▄▄▄▄▄▄▀▀▀▀▀▀ ▀▀▀▀▀▀▀▀▀▀▀ 
▐░▌             ▐░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░▌         ▐░░░░░░░░░░░▐░░░░░░░░░░░▌                  
 ▐░▌           ▐░▌▐░█▀▀▀▀▀▀▀▀▀▐░█▀▀▀▀▀▀▀█░▌▀▀▀▀█░█▀▀▀▀▐░▌         ▐░█▀▀▀▀▀▀▀█░▐░█▀▀▀▀▀▀▀▀▀                   
  ▐░▌         ▐░▌ ▐░▌         ▐░▌       ▐░▌    ▐░▌    ▐░▌         ▐░▌       ▐░▐░▌                            
   ▐░▌       ▐░▌  ▐░█▄▄▄▄▄▄▄▄▄▐░█▄▄▄▄▄▄▄█░▌    ▐░▌    ▐░▌         ▐░▌       ▐░▐░▌ ▄▄▄▄▄▄▄▄                   
    ▐░▌     ▐░▌   ▐░░░░░░░░░░░▐░░░░░░░░░░░▌    ▐░▌    ▐░▌         ▐░▌       ▐░▐░▌▐░░░░░░░░▌                  
     ▐░▌   ▐░▌    ▐░█▀▀▀▀▀▀▀▀▀▐░█▀▀▀▀█░█▀▀     ▐░▌    ▐░▌         ▐░▌       ▐░▐░▌ ▀▀▀▀▀▀█░▌                  
      ▐░▌ ▐░▌     ▐░▌         ▐░▌     ▐░▌      ▐░▌    ▐░▌         ▐░▌       ▐░▐░▌       ▐░▌                  
       ▐░▐░▌      ▐░█▄▄▄▄▄▄▄▄▄▐░▌      ▐░▌ ▄▄▄▄█░█▄▄▄▄▐░█▄▄▄▄▄▄▄▄▄▐░█▄▄▄▄▄▄▄█░▐░█▄▄▄▄▄▄▄█░▌                  
        ▐░▌       ▐░░░░░░░░░░░▐░▌       ▐░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░░░░░░░░░░░▐░░░░░░░░░░░▌                  
         ▀         ▀▀▀▀▀▀▀▀▀▀▀ ▀         ▀ ▀▀▀▀▀▀▀▀▀▀▀ ▀▀▀▀▀▀▀▀▀▀▀ ▀▀▀▀▀▀▀▀▀▀▀ ▀▀▀▀▀▀▀▀▀▀▀                   
                                                                                                             
```

一款基于Vimscript的自动化verilog脚本。由[automatic for Verilog & RtlTree](https://www.vim.org/scripts/script.php?script_id=4067)修改而来，原作者zhangguo。

[![Release-Version](https://img.shields.io/badge/Release-1.0.3-blue.svg)](https://github.com/HonkW93/automatic-verilog/releases)-[![Vim-Version](https://img.shields.io/badge/Vim-8.2-green.svg)](https://www.vim.org/download.php)

## 安装

将automatic.vim放入vim根目录下的plugin文件夹即可。

**提示：此脚本可能会修改文本数据，请在使用前备份数据，防止数据覆盖等情况发生。**

 ## 特性

- 自动例化（`AutoInst`）
  - [x] 支持跨文件夹搜索.v文件进行例化，支持文件夹递归（参考`emacs verilog-mode`）
  - [x] 支持端口重刷（参考`emacs verilog-mode`）
  - [x] 支持行尾自动添加端口类型`input/output/inout` （参考`vim automatic-verilog`）
  - [x] 支持新增端口自动添加`//INST_NEW`（参考`vim automatic-verilog`）
  - [x] 支持删除端口自动添加`//INST_DEL`（参考`vim automatic-verilog`）
  - [ ] 支持`` `ifdef``及`` `endif``
  - [ ] 进行中...
  
- 自动参数（`AutoPara`）
  - [x] 支持跨文件夹搜索.v文件进行例化，支持文件夹递归（参考`emacs verilog-mode`）
  - [x] 支持参数重刷（参考`emacs verilog-mode`）
  - [x] 支持新增端口自动添加`//PARA_NEW`（参考`vim automatic-verilog`）
  - [x] 支持删除端口自动添加`//PARA_DEL`（参考`vim automatic-verilog`）
  - [x] 支持`parameter`连续多个的写法，例如`parameter A = 1, B = 5, C = 6`
  - [ ] 支持`` `ifdef``及`` `endif``
  - [ ] 进行中...
  
- 自动reg（`AutoReg`）
  - [ ] 支持端口`output reg`覆盖定义（参考`emacs verilog-mode`）
  - [ ] 支持`always`语句阻塞/非阻塞赋值`reg`获取（参考`vim automatic-verilog`）
    - [x] 支持左端`{}`写法，但不支持此写法获取位宽
    - [x] 支持左端`[WIDTH1:WIDTH2]`写法
    - [x] 支持右端`16'd1`或 `2'b01`或 `4'hf`或```WIDTH'hf``写法
    - [x] 支持右端`[WIDTH-1:0]`或 `[2*3-1:0]`或`[WIDTH1:WIDTH2]`写法
    - [x] 支持右端`signal_a`或 `~signal_a`或`！signal_a`写法
    - [x] 支持右端`signal_a & signal_b | signal_c[2:0]`写法
    - [x] 支持右端`en ? signal_b : signal_c[2:0]`写法
    - [x] 支持右端`{}`写法
    - [ ] 进行中...
  
- 自动wire（`AutoWire`）
  - [ ] 支持例化`inst_wire`自动获取
  - [ ] 支持`assign`语句`wire`自动获取
  - [ ] 进行中...

- 自动定义（`AutoDef`） 
  - [ ] 支持`AutoWire`
  - [ ] 支持`AutoReg`
  - [ ] 进行中...

- 自动接口（`AutoInterface`）
  - [ ] 梳理`sv`中`interface`的自动例化
  - [ ] 梳理中...

- 其他（`Other`）
 - [ ] 梳理`emacs verilog-mode`中其他`auto`函数...
 - [ ] 梳理中...

## 文档

[Vimcript-AutoMatic | HonkW](https://blog.honk.wang/posts/AutoMatic/)


## 开源协议

[GPL V3.0](/LICENSE)
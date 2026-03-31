+++
title = 'Assembly Word'
date = 2026-03-03T19:26:59-07:00
draft = false
+++

在 x86 体系里——不管 16 位、32 位、还是 64 位模式——
WORD 永远是 16 位 = 2 字节。
这是历史遗产。
早期 8086 是 16 位 CPU。
当时“word”就是机器的自然数据宽度——16 位。
后来扩展到 32 位：
原来的 word 仍然是 16 位
新的 32 位被叫做 double word（DWORD）
再到 64 位：
64 位叫 quad word（QWORD）
所以单位一直叠加：
BYTE = 8 bit
WORD = 16 bit
DWORD = 32 bit
QWORD = 64 bit

这里的“double”不是“相对当前模式”，
而是相对最初的 16 位 word。
# Comparing `tmp/seclm-0.0.1-py3-none-any.whl.zip` & `tmp/seclm-0.1.0.tar.gz`

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  tmp/seclm-0.1.0.tar.gz*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,71 +1,134 @@
-00000000: 504b 0304 1400 0000 0800 cf32 7d58 0000  PK.........2}X..
-00000010: 0000 0200 0000 0000 0000 1100 0000 7365  ..............se
-00000020: 636c 6d2f 5f5f 696e 6974 5f5f 2e70 7903  clm/__init__.py.
-00000030: 0050 4b03 0414 0000 0008 0004 069a 5861  .PK...........Xa
-00000040: 512b 5e6c 0000 007e 0000 001e 0000 0073  Q+^l...~.......s
-00000050: 6563 6c6d 2d30 2e30 2e31 2e64 6973 742d  eclm-0.0.1.dist-
-00000060: 696e 666f 2f4d 4554 4144 4154 41f3 4d2d  info/METADATA.M-
-00000070: 494c 492c 49d4 0d4b 2d2a cecc cfb3 5230  ILI,I..K-*....R0
-00000080: d233 e4f2 4bcc 4db5 5228 4e4d cec9 e582  .3..K.M.R(NM....
-00000090: 4b18 e819 00a5 824b 7373 138b 2a61 b21e  K......Kss..*a..
-000000a0: f9b9 a9ba 0589 e940 e519 2525 05c5 56fa  .......@..%%..V.
-000000b0: fae9 9925 19a5 497a c9f9 b9fa 4035 ba40  ...%..Iz....@5.@
-000000c0: 4541 a985 a599 45a9 c5ba 0195 2519 20a3  EA....E.....%. .
-000000d0: ec6c 8df5 0c0d b8b8 0050 4b03 0414 0000  .l.......PK.....
-000000e0: 0008 0004 069a 58fc 0e7b 4b5c 0000 005c  ......X..{K\...\
-000000f0: 0000 001b 0000 0073 6563 6c6d 2d30 2e30  .......seclm-0.0
-00000100: 2e31 2e64 6973 742d 696e 666f 2f57 4845  .1.dist-info/WHE
-00000110: 454c 0bcf 484d cdd1 0d4b 2d2a cecc cfb3  EL..HM...K-*....
-00000120: 5230 d433 e072 4fcd 4b2d 4a2c c92f b252  R0.3.rO.K-J,./.R
-00000130: 484a c92c 2e89 2f07 a951 d030 d033 31d6  HJ.,../..Q.0.31.
-00000140: 33d0 e40a cacf 2fd1 f52c d60d 282d 4acd  3...../..,..(-J.
-00000150: c94c b252 2829 2a4d e50a 494c b752 28a8  .L.R()*M..IL.R(.
-00000160: 34d6 cdcb cf4b d54d ccab e4e2 0200 504b  4....K.M......PK
-00000170: 0304 1400 0000 0800 0406 9a58 acb0 7e35  ...........X..~5
-00000180: 0800 0000 0600 0000 2300 0000 7365 636c  ........#...secl
-00000190: 6d2d 302e 302e 312e 6469 7374 2d69 6e66  m-0.0.1.dist-inf
-000001a0: 6f2f 746f 705f 6c65 7665 6c2e 7478 742b  o/top_level.txt+
-000001b0: 4e4d cec9 e502 0050 4b03 0414 0000 0008  NM.....PK.......
-000001c0: 0004 069a 5824 9edc ebfa 0000 0067 0100  ....X$.......g..
-000001d0: 001c 0000 0073 6563 6c6d 2d30 2e30 2e31  .....seclm-0.0.1
-000001e0: 2e64 6973 742d 696e 666f 2f52 4543 4f52  .dist-info/RECOR
-000001f0: 4475 ce4b 7282 3000 00d0 bd67 4910 5110  Du.Kr.0....gI.Q.
-00000200: 165d 207f 151c 3048 eb26 0336 c528 5f09  .] ...0H.&.6.(_.
-00000210: 047a fa4e 172c bdc0 9bd7 915b 512e 31a6  .z.N.,.....[Q.1.
-00000220: 1565 180b cd04 ba7b 2ac9 cac7 666b 5a61  .e.....{*...fkZa
-00000230: f350 dddd 3985 1879 6502 e5bd 41fa 9044  .P..9..ye...A..D
-00000240: cf52 0efc 669f 5c9d f5fd dcdb 3110 17dd  .R..f.\.....1...
-00000250: 3f03 4541 1456 c237 ed18 a4d5 4fbd f42d  ?.EA.V.7....O..-
-00000260: a49b 3ad2 6733 1f22 aef3 6c3d bd54 625a  ..:.g3."..l=.TbZ
-00000270: 7d2c b551 96e7 d722 88a8 e9d8 f7de f33c  },.Q...".......<
-00000280: fe70 434a 9a2f b092 9437 6ae2 5ad6 7126  .pCJ./...7j.Z.q&
-00000290: 9dfd 96e1 67b2 b327 9ea5 f941 26b5 e6d5  ....g..'...A&...
-000002a0: 313f 264a 3d9d 083a 9421 d4a8 6b5f 8231  1?&J=..:.!..k_.1
-000002b0: 049a f446 6475 830b 3290 4260 239b 65d4  ...Fdu..2.B`#.e.
-000002c0: 429c 8f1b fe6c 6bf3 f3b7 1a52 d1a8 2e63  B....lk....R...c
-000002d0: 962a 1e42 b783 c3ae f9e9 75ec 3415 6e7d  .*.B......u.4.n}
-000002e0: f0ae 1a59 c629 3201 58fc 0150 4b01 0214  ...Y.)2.X..PK...
-000002f0: 0314 0000 0008 00cf 327d 5800 0000 0002  ........2}X.....
-00000300: 0000 0000 0000 0011 0000 0000 0000 0000  ................
-00000310: 0000 00b4 8100 0000 0073 6563 6c6d 2f5f  .........seclm/_
-00000320: 5f69 6e69 745f 5f2e 7079 504b 0102 1403  _init__.pyPK....
-00000330: 1400 0000 0800 0406 9a58 6151 2b5e 6c00  .........XaQ+^l.
-00000340: 0000 7e00 0000 1e00 0000 0000 0000 0000  ..~.............
-00000350: 0000 b481 3100 0000 7365 636c 6d2d 302e  ....1...seclm-0.
-00000360: 302e 312e 6469 7374 2d69 6e66 6f2f 4d45  0.1.dist-info/ME
-00000370: 5441 4441 5441 504b 0102 1403 1400 0000  TADATAPK........
-00000380: 0800 0406 9a58 fc0e 7b4b 5c00 0000 5c00  .....X..{K\...\.
-00000390: 0000 1b00 0000 0000 0000 0000 0000 b481  ................
-000003a0: d900 0000 7365 636c 6d2d 302e 302e 312e  ....seclm-0.0.1.
-000003b0: 6469 7374 2d69 6e66 6f2f 5748 4545 4c50  dist-info/WHEELP
-000003c0: 4b01 0214 0314 0000 0008 0004 069a 58ac  K.............X.
-000003d0: b07e 3508 0000 0006 0000 0023 0000 0000  .~5........#....
-000003e0: 0000 0000 0000 00a4 816e 0100 0073 6563  .........n...sec
-000003f0: 6c6d 2d30 2e30 2e31 2e64 6973 742d 696e  lm-0.0.1.dist-in
-00000400: 666f 2f74 6f70 5f6c 6576 656c 2e74 7874  fo/top_level.txt
-00000410: 504b 0102 1403 1400 0000 0800 0406 9a58  PK.............X
-00000420: 249e dceb fa00 0000 6701 0000 1c00 0000  $.......g.......
-00000430: 0000 0000 0000 0000 b481 b701 0000 7365  ..............se
-00000440: 636c 6d2d 302e 302e 312e 6469 7374 2d69  clm-0.0.1.dist-i
-00000450: 6e66 6f2f 5245 434f 5244 504b 0506 0000  nfo/RECORDPK....
-00000460: 0000 0500 0500 6f01 0000 eb02 0000 0000  ......o.........
+00000000: 1f8b 0808 0a81 3466 02ff 7365 636c 6d2d  ......4f..seclm-
+00000010: 302e 312e 302e 7461 7200 ed5d 6b6f e336  0.1.0.tar..]ko.6
+00000020: 16cd 67fd 0ac2 f3c1 3610 cb7a db0e a045  ..g.....6..z...E
+00000030: b333 994d d079 04c9 b468 5114 1a5a a66d  .3.M.y...hQ..Z.m
+00000040: eee8 b522 9dc6 2dfa df7b 4949 8ee3 c903  ..."..-..{II....
+00000050: 03c4 5ab4 be07 3391 78f9 10c5 c73d 97d4  ..Z...3.x....=..
+00000060: 9565 0ecd e177 97f4 f69c d119 2b8f f602  .e...w......+...
+00000070: abc2 6347 cb72 bdbb 7325 b72d c776 8ec8  ..cG.r..s%.-.v..
+00000080: ed51 0b58 0949 4bb8 fcd1 61c2 1993 54f2  .Q.X.IK...a...T.
+00000090: 9485 f6c8 f646 7630 71c7 a617 f8b6 ed7a  .....Fv0q......z
+000000a0: c611 e21f 0fc1 e224 1d58 a66d 5ac3 7d5d  .......$.X.mZ.}]
+000000b0: 434d ead1 c857 4777 e458 dbc7 cd9c b7bd  CM...WGw.X......
+000000c0: c0f6 6dcb f260 e25b b6e3 38ee 11f1 db9c  ..m..`.[..8.....
+000000d0: ff42 662c 5b3c d150 cfc4 ff4d 61a2 fe47  .Bf,[<.P...Ma..G
+000000e0: fd8f fa1f f53f e8ff cbef ff33 b8f8 f0f6  .....?.....3....
+000000f0: e33e e67f e079 8fea 7fd7 7677 f4bf ab44  .>...y....vw...D
+00000100: c46a 73fe 1fa8 fe7f cf24 9d51 4907 3fb2  .js......$.QI.?.
+00000110: 52f0 3c3b 218e 691b 1f68 ca4e 881e 1bc6  R.<;!.i..h.N....
+00000120: 2642 0f12 e37a 95a6 b45c 37b1 e779 ca06  &B...z...\7..y..
+00000130: 055d 40f2 a594 8538 190e 175c 2e57 5333  .]@....8...\.WS3
+00000140: ced3 21a4 1924 fa00 494f 5772 9997 9051  ..!..$..IOWr...Q
+00000150: b764 1d1c b094 f2e4 8440 a6ef aa08 95d1  .d.......@......
+00000160: b862 ff5b f192 89c1 e51a 52c1 c5ff 15ba  .b.[......R.....
+00000170: a66d ddc9 df70 214f 485c ae0b 992f 4a5a  .m...p!OH\.../JZ
+00000180: 2cd7 a8ae feb6 fcef 045f f3bf 8bfc df0a  ,........_......
+00000190: ff3b f7f9 3f98 8c60 92e3 bc38 44fe bf3a  .;..?..`...8D..:
+000001a0: 3b7d f3fe cc4c 67fb e0ff e051 fe87 c59e  ;}...Lg....Q....
+000001b0: b7e1 7f30 0614 ff7b a311 f27f 1b78 45ae  ...0...{.....xE.
+000001c0: 59fc ee3d 49f8 b404 5a37 3e2d b968 02a4  Y..=I...Z7>-.h..
+000001d0: 28f3 1b3e 6382 c479 76c3 32ce 3249 681c  (..>c..yv.2.2Ih.
+000001e0: 3321 88cc 49c1 3342 3372 7dfd 8ec4 ac94  3!..I.3B3r}.....
+000001f0: 7cce 632a 998a a144 142c 5602 52ac a65f  |.c*...D.,V.R.._
+00000200: d8da 348c 57af c845 066d 9d24 5482 3961  ..4.W..E.m.$T.9a
+00000210: 7cfe fcd9 2878 4178 25ac cd09 2555 497f  |...(xAx%...%UI.
+00000220: 1060 5218 e7ac 6484 c27f 0156 0661 b734  .`R...d....V.a.4
+00000230: 2d12 a84d 3e27 2bc1 b305 e112 b293 199f  -..M>'+.........
+00000240: cf21 21d4 adaa 3767 c254 0515 da74 305e  .!!...7g.T...t0^
+00000250: d595 5993 5599 4085 6744 2ca9 e307 c6bc  ..Y.U.@.gD,.....
+00000260: ccd3 eab2 a610 09e1 6991 9712 4c0a 0677  ........i...L..w
+00000270: 1181 2482 bb96 ec56 1a5b e724 7c20 41af  ..$....V.[.$| A.
+00000280: d398 3e75 15cd aa54 3064 3ac7 a433 61c1  ..>u...T0d:..3a.
+00000290: c499 04d3 7930 1edb fed8 9d30 279e fbb1  ....y0.....0'...
+000002a0: eb78 ae3d 9ebb 9637 a563 3a9a 3167 ee8f  .x.=...7.c:.1g..
+000002b0: 478e e7c7 563c 1df9 73df 63ee 9cd9 93a0  G...V<..s.c.....
+000002c0: d387 26d1 d6d5 ad51 57b2 0ae8 bfe6 823d  ..&....QW......=
+000002d0: 5381 1b56 c2dd 875b 15d6 0552 9eab 5c4d  S..V...[...R..\M
+000002e0: 9154 acb3 98e7 9b60 1dab c564 c6e6 04ec  .T.....`...d....
+000002f0: b4ac d73f 3108 a092 fe06 865e 93d0 7c9d  ...?1......^..|.
+00000300: a8e1 710d 6303 7ab7 d787 24d0 b63a 5065  ..q.c.z...$..:Pe
+00000310: d9c9 56c7 3d5f 7ba8 f6bd aaab 82c1 002c  ..V.=_{........,
+00000320: f24c b0bb 9275 e9bf 5118 104d 9ca9 7ba6  .L...u..Q..M..{.
+00000330: 6fd4 f765 96ab ac57 dd82 befb bc60 19e5  o..e...W.....`..
+00000340: d518 a8ce 9b01 f011 42a7 17c7 e40d 9bd3  ........B.......
+00000350: 5522 cf55 2357 3767 c4fa 0063 a04a d3ab  U".U#W7g...c.J..
+00000360: daa2 e011 0cf1 b073 f6fe f2d3 cf9d 632d  .......s......c-
+00000370: 9c52 c122 186f e1e3 f736 bcb1 ebc4 2a49  .R.".o...6....*I
+00000380: 5495 1d7e 7dd5 de43 fdd7 37e2 2595 1056  T..~}..C..7.%..V
+00000390: 65aa f9a4 06a6 4e6e aa08 f32e 4298 d580  e.....Nn....B...
+000003a0: ad2a 9b42 b3c3 cc12 e12f 9ba6 fbe3 5e23  .*.B...../....^#
+000003b0: 76ca 3c61 9d13 d259 0956 d6f5 dbc4 e9cb  v.<a...Y.V......
+000003c0: 6752 455f d335 914a 57c0 3f4a 2413 722b  gRE_.5.JW.?J$.r+
+000003d0: f19f faec d74a 90e6 3306 ed90 c242 6300  .....J..3....Bc.
+000003e0: 933f a543 b5e6 18bc 53a7 0377 30fe f740  .?.C....S..w0..@
+000003f0: e985 7215 ab12 fa6a e222 2be3 fe1f eeff  ..r....j."+.....
+00000400: e1fe 1fa2 5dfb 5f9f 0ff7 33ff bfed f98f  ....]._...3.....
+00000410: eb3a 013e ffc1 fd1f d4ff edee ff58 93c0  .:.>.........X..
+00000420: 9be0 fecf 41eb ff28 e219 9751 6416 eb76  ....A..(...Qd..v
+00000430: f67f eef4 bf15 388e a3f6 7f7c cf75 70ff  ......8....|.up.
+00000440: 07ed 7fd4 ff68 ff23 dad5 ff42 24c3 979f  .....h.#...B$...
+00000450: ffdf 66ff c3df 11da ff68 ffa3 fe6f d7fe  ..f......h...o..
+00000460: b72d d7b6 d0fe 3f78 fdff b26b 8067 ed7f  .-....?x...k.g..
+00000470: 7f63 ffbb 9e07 bac0 0e1c 1fed ff56 a01f  .c...........V..
+00000480: 8099 cdd3 cdc7 9f81 e24c f967 02f9 1ff9  .........L.g....
+00000490: 7f8b ff5d cbc2 fd3f e4ff 5aeb bfd0 16e0  ...]...?..Z.....
+000004a0: 33fc 6f07 6e50 f3ff 08d2 d99a ff2d f4ff  3.o.nP.......-..
+000004b0: 6a8f ffb7 dda8 cd5b df9a 3486 4092 d359  j......[..4.@..Y
+000004c0: 54b0 3452 c268 cbcb cbf8 3adf 92fe 9e52  T.4R.h....:....R
+000004d0: 1832 254f b9e4 374c 3485 0856 729a f0df  .2%O..7L4..Vr...
+000004e0: 2bbf afc6 8389 8a65 c2a7 4d10 065d 55e4  +......e..M..]U.
+000004f0: aa4c 406c 16b4 14ac 2900 643a 6c18 8672  .L@l....).d:l..r
+00000500: 447a c001 0b52 28bf f2f2 b8f6 edd2 0112  Dz...R(.........
+00000510: 920f 79c6 6a97 a512 2a14 6e8a 5239 fa95  ..y.j...*.n.R9..
+00000520: f34d 2e94 470f 449b ea34 a329 d372 7de5  .M..G.D..4.).r}.
+00000530: 9078 9e4b f85c 4757 92aa 50c2 12a8 5f23  .x.K.\GW..P..._#
+00000540: d519 54eb a8b6 824c 5035 e5d8 14c1 9ddf  ..T....LP5......
+00000550: b072 bbdd 7a3d 7591 635d 7abf bfc9 0779  .r..z=u.c]z....y
+00000560: 1e6d ea5e 53b0 c9b2 389f b15e 7725 e783  .m.^S...8..^w%..
+00000570: 71b7 ce5e 39d8 45d3 b5d4 37a8 129b 204b  q..^9.E...7... K
+00000580: 78ac bc92 7afd 26a0 13f4 7411 3c5b 84f7  x...z.&...t.<[..
+00000590: 3ac5 3cab c5e6 9bb3 ab63 32cf 4be8 c99d  :.<......c2.K...
+000005a0: 2497 ba98 b73a cabc 5e4d ffcb 6259 c9be  $....:..^M..bY..
+000005b0: 67eb 8b6c 9edf ab4e d50d 509f ba9f cd4a  g..l...N..P....J
+000005c0: d0db ae6d df5c b2db 195f 30a1 fcb4 5466  ...m.\..._0...Tf
+000005d0: 68e8 3a23 1724 cba5 6eea 6df7 31a1 da6a  h.:#.$..n.m.1..j
+000005e0: e712 61e3 cfa7 1b73 e3a6 a7fa a01e 29b3  ..a....s......).
+000005f0: caa7 6a33 5a62 fdc6 43d8 b46b dfd8 2abc  ..j3Zb..C..k..*.
+00000600: d17c 3a52 c8bc 8481 26a9 14bd beba d21f  .|:R....&.......
+00000610: 5dd5 3bdd 1362 1f93 6e5c 2670 66c1 59d5  ].;..b..n\&pf.Y.
+00000620: 6554 85fe dcae 8659 b96e 45f3 842e 445d  eT.....Y.nE...D]
+00000630: a71f cfae 2ede fe1c fda4 b25c 9e5e 7dba  ...........\.^}.
+00000640: 387d 17bd 3e3f bdf8 508f 52b9 2a33 d29e  8}..>?..P.R.*3..
+00000650: d58d fbff b8ff 8ffb ff68 ff6d ec3f 932d  .........h.m.?.-
+00000660: 1603 0efa 7cf8 a2f3 ffdb f6ff 7d0b a271  ....|.......}..q
+00000670: ff1f d7ff a8ff db5d ff6b fd8f eb7f d4ff  .......].k......
+00000680: a0ff 5fec 75f0 6f7f ff3b b06d 0bd7 ff6d  .._.u.o..;.m...m
+00000690: 00df ff3e 6c20 ff23 ff23 ff23 ff3f c0ff  ...>l .#.#.#.?..
+000006a0: d71f 7fb8 7a7d 766d ca5b f902 fcff c4f3  ....z}vm.[......
+000006b0: 7fd7 1ded f2ff 08f7 ffdb c1e6 9d7f 4330  ..............C0
+000006c0: b92a cc62 6d7c e506 6e3c 6218 1a8f 0f98  .*.bm|..n<b.....
+000006d0: dda8 192b 5836 6359 bc8e 129e 7d11 0fa5  ...+X6cY....}...
+000006e0: 296b 6e7f 284e e645 94b0 1b96 dc45 ee3a  )kn.(N.E.....E.:
+000006f0: aa18 fb7a 7c85 fc8f fc8f fc8f 3834 fe7f  ...z|.......84..
+00000700: 4867 ef85 ff2d cbbe cfff 8e0d e991 ffdb  Hg...-..........
+00000710: 004e 75e4 7fe4 7fe4 7fe4 7fe4 ff27 d663  .Nu..........'.c
+00000720: 7b5d ff5b b6bf b3fe 1f79 b687 fcdf 0670  {].[.....y.....p
+00000730: 071d f91f f91f f91f f91f f9ff a93d d7bd  .............=..
+00000740: f2bf 15ec f2bf efe1 fabf bdfe c7f9 8efc  ................
+00000750: 8ffe df87 c9ff e8ff 8dfc bfe1 7ff5 0438  ...............8
+00000760: 9e2f f630 ff9f e47f 6f97 ff3d cbc3 f57f  ./.0....o..=....
+00000770: 2bf8 05cc bd48 997b bf1a 922e a2e9 8a27  +....H.{.......'
+00000780: 3312 121d 98a9 9f73 0f89 65a0 2640 fec7  3......s..e.&@..
+00000790: f5ff 21ac ff2d 6fec e3fa ffa0 f9ff e59d  ..!..-o.........
+000007a0: a69e e37f df72 36bf ff33 727c f5fb cf23  .....r6..3r|...#
+000007b0: df46 fe6f 03f5 4750 a0e3 659e 275b efec  .F.o..GP..e.'[..
+000007c0: 83c4 a87c 02ab 2f47 a817 e3c3 ae1e 2edd  ...|../G........
+000007d0: eac3 0e37 d58b 0161 578f 9e5a 3863 222e  ...7...aW..Z8c".
+000007e0: 7921 75c4 766a aadd fd41 a6db f19e 30d2  y!u.vj...A....0.
+000007f0: ef00 84dd fbef 00d4 49d4 4734 bacf bc5a  ........I.G4...Z
+00000800: 5027 2d68 fca5 fab8 4573 65d2 dd7c dfa5  P'-h....Ese..|..
+00000810: 5b7f 8ea2 fede 4cd4 3cdd dafa 1246 77fb  [.....L.<....Fw.
+00000820: 6148 77fb 1b16 d5a7 64ee f274 abd7 11ba  aHw.....d..t....
+00000830: ea83 15a8 4310 0804 0281 4020 1008 0402  ....C.....@ ....
+00000840: 8140 2010 0804 0281 4020 1008 0402 8140  .@ .....@ .....@
+00000850: 2010 08c4 ff07 7f01 eec8 574f 00a0 0000   .........WO....
```

## Comparing `tmp/seclm-0.0.1-py3-none-any.whl.zip` & `tmp/seclm-0.1.0.tar.gz`

```diff
@@ -1,71 +1,134 @@
-00000000: 504b 0304 1400 0000 0800 cf32 7d58 0000  PK.........2}X..
-00000010: 0000 0200 0000 0000 0000 1100 0000 7365  ..............se
-00000020: 636c 6d2f 5f5f 696e 6974 5f5f 2e70 7903  clm/__init__.py.
-00000030: 0050 4b03 0414 0000 0008 0004 069a 5861  .PK...........Xa
-00000040: 512b 5e6c 0000 007e 0000 001e 0000 0073  Q+^l...~.......s
-00000050: 6563 6c6d 2d30 2e30 2e31 2e64 6973 742d  eclm-0.0.1.dist-
-00000060: 696e 666f 2f4d 4554 4144 4154 41f3 4d2d  info/METADATA.M-
-00000070: 494c 492c 49d4 0d4b 2d2a cecc cfb3 5230  ILI,I..K-*....R0
-00000080: d233 e4f2 4bcc 4db5 5228 4e4d cec9 e582  .3..K.M.R(NM....
-00000090: 4b18 e819 00a5 824b 7373 138b 2a61 b21e  K......Kss..*a..
-000000a0: f9b9 a9ba 0589 e940 e519 2525 05c5 56fa  .......@..%%..V.
-000000b0: fae9 9925 19a5 497a c9f9 b9fa 4035 ba40  ...%..Iz....@5.@
-000000c0: 4541 a985 a599 45a9 c5ba 0195 2519 20a3  EA....E.....%. .
-000000d0: ec6c 8df5 0c0d b8b8 0050 4b03 0414 0000  .l.......PK.....
-000000e0: 0008 0004 069a 58fc 0e7b 4b5c 0000 005c  ......X..{K\...\
-000000f0: 0000 001b 0000 0073 6563 6c6d 2d30 2e30  .......seclm-0.0
-00000100: 2e31 2e64 6973 742d 696e 666f 2f57 4845  .1.dist-info/WHE
-00000110: 454c 0bcf 484d cdd1 0d4b 2d2a cecc cfb3  EL..HM...K-*....
-00000120: 5230 d433 e072 4fcd 4b2d 4a2c c92f b252  R0.3.rO.K-J,./.R
-00000130: 484a c92c 2e89 2f07 a951 d030 d033 31d6  HJ.,../..Q.0.31.
-00000140: 33d0 e40a cacf 2fd1 f52c d60d 282d 4acd  3...../..,..(-J.
-00000150: c94c b252 2829 2a4d e50a 494c b752 28a8  .L.R()*M..IL.R(.
-00000160: 34d6 cdcb cf4b d54d ccab e4e2 0200 504b  4....K.M......PK
-00000170: 0304 1400 0000 0800 0406 9a58 acb0 7e35  ...........X..~5
-00000180: 0800 0000 0600 0000 2300 0000 7365 636c  ........#...secl
-00000190: 6d2d 302e 302e 312e 6469 7374 2d69 6e66  m-0.0.1.dist-inf
-000001a0: 6f2f 746f 705f 6c65 7665 6c2e 7478 742b  o/top_level.txt+
-000001b0: 4e4d cec9 e502 0050 4b03 0414 0000 0008  NM.....PK.......
-000001c0: 0004 069a 5824 9edc ebfa 0000 0067 0100  ....X$.......g..
-000001d0: 001c 0000 0073 6563 6c6d 2d30 2e30 2e31  .....seclm-0.0.1
-000001e0: 2e64 6973 742d 696e 666f 2f52 4543 4f52  .dist-info/RECOR
-000001f0: 4475 ce4b 7282 3000 00d0 bd67 4910 5110  Du.Kr.0....gI.Q.
-00000200: 165d 207f 151c 3048 eb26 0336 c528 5f09  .] ...0H.&.6.(_.
-00000210: 047a fa4e 172c bdc0 9bd7 915b 512e 31a6  .z.N.,.....[Q.1.
-00000220: 1565 180b cd04 ba7b 2ac9 cac7 666b 5a61  .e.....{*...fkZa
-00000230: f350 dddd 3985 1879 6502 e5bd 41fa 9044  .P..9..ye...A..D
-00000240: cf52 0efc 669f 5c9d f5fd dcdb 3110 17dd  .R..f.\.....1...
-00000250: 3f03 4541 1456 c237 ed18 a4d5 4fbd f42d  ?.EA.V.7....O..-
-00000260: a49b 3ad2 6733 1f22 aef3 6c3d bd54 625a  ..:.g3."..l=.TbZ
-00000270: 7d2c b551 96e7 d722 88a8 e9d8 f7de f33c  },.Q...".......<
-00000280: fe70 434a 9a2f b092 9437 6ae2 5ad6 7126  .pCJ./...7j.Z.q&
-00000290: 9dfd 96e1 67b2 b327 9ea5 f941 26b5 e6d5  ....g..'...A&...
-000002a0: 313f 264a 3d9d 083a 9421 d4a8 6b5f 8231  1?&J=..:.!..k_.1
-000002b0: 049a f446 6475 830b 3290 4260 239b 65d4  ...Fdu..2.B`#.e.
-000002c0: 429c 8f1b fe6c 6bf3 f3b7 1a52 d1a8 2e63  B....lk....R...c
-000002d0: 962a 1e42 b783 c3ae f9e9 75ec 3415 6e7d  .*.B......u.4.n}
-000002e0: f0ae 1a59 c629 3201 58fc 0150 4b01 0214  ...Y.)2.X..PK...
-000002f0: 0314 0000 0008 00cf 327d 5800 0000 0002  ........2}X.....
-00000300: 0000 0000 0000 0011 0000 0000 0000 0000  ................
-00000310: 0000 00b4 8100 0000 0073 6563 6c6d 2f5f  .........seclm/_
-00000320: 5f69 6e69 745f 5f2e 7079 504b 0102 1403  _init__.pyPK....
-00000330: 1400 0000 0800 0406 9a58 6151 2b5e 6c00  .........XaQ+^l.
-00000340: 0000 7e00 0000 1e00 0000 0000 0000 0000  ..~.............
-00000350: 0000 b481 3100 0000 7365 636c 6d2d 302e  ....1...seclm-0.
-00000360: 302e 312e 6469 7374 2d69 6e66 6f2f 4d45  0.1.dist-info/ME
-00000370: 5441 4441 5441 504b 0102 1403 1400 0000  TADATAPK........
-00000380: 0800 0406 9a58 fc0e 7b4b 5c00 0000 5c00  .....X..{K\...\.
-00000390: 0000 1b00 0000 0000 0000 0000 0000 b481  ................
-000003a0: d900 0000 7365 636c 6d2d 302e 302e 312e  ....seclm-0.0.1.
-000003b0: 6469 7374 2d69 6e66 6f2f 5748 4545 4c50  dist-info/WHEELP
-000003c0: 4b01 0214 0314 0000 0008 0004 069a 58ac  K.............X.
-000003d0: b07e 3508 0000 0006 0000 0023 0000 0000  .~5........#....
-000003e0: 0000 0000 0000 00a4 816e 0100 0073 6563  .........n...sec
-000003f0: 6c6d 2d30 2e30 2e31 2e64 6973 742d 696e  lm-0.0.1.dist-in
-00000400: 666f 2f74 6f70 5f6c 6576 656c 2e74 7874  fo/top_level.txt
-00000410: 504b 0102 1403 1400 0000 0800 0406 9a58  PK.............X
-00000420: 249e dceb fa00 0000 6701 0000 1c00 0000  $.......g.......
-00000430: 0000 0000 0000 0000 b481 b701 0000 7365  ..............se
-00000440: 636c 6d2d 302e 302e 312e 6469 7374 2d69  clm-0.0.1.dist-i
-00000450: 6e66 6f2f 5245 434f 5244 504b 0506 0000  nfo/RECORDPK....
-00000460: 0000 0500 0500 6f01 0000 eb02 0000 0000  ......o.........
+00000000: 1f8b 0808 0a81 3466 02ff 7365 636c 6d2d  ......4f..seclm-
+00000010: 302e 312e 302e 7461 7200 ed5d 6b6f e336  0.1.0.tar..]ko.6
+00000020: 16cd 67fd 0ac2 f3c1 3610 cb7a db0e a045  ..g.....6..z...E
+00000030: b333 994d d079 04c9 b468 5114 1a5a a66d  .3.M.y...hQ..Z.m
+00000040: eee8 b522 9dc6 2dfa df7b 4949 8ee3 c903  ..."..-..{II....
+00000050: 03c4 5ab4 be07 3391 78f9 10c5 c73d 97d4  ..Z...3.x....=..
+00000060: 9565 0ecd e177 97f4 f69c d119 2b8f f602  .e...w......+...
+00000070: abc2 6347 cb72 bdbb 7325 b72d c776 8ec8  ..cG.r..s%.-.v..
+00000080: ed51 0b58 0949 4bb8 fcd1 61c2 1993 54f2  .Q.X.IK...a...T.
+00000090: 9485 f6c8 f646 7630 71c7 a617 f8b6 ed7a  .....Fv0q......z
+000000a0: c611 e21f 0fc1 e224 1d58 a66d 5ac3 7d5d  .......$.X.mZ.}]
+000000b0: 434d ead1 c857 4777 e458 dbc7 cd9c b7bd  CM...WGw.X......
+000000c0: c0f6 6dcb f260 e25b b6e3 38ee 11f1 db9c  ..m..`.[..8.....
+000000d0: ff42 662c 5b3c d150 cfc4 ff4d 61a2 fe47  .Bf,[<.P...Ma..G
+000000e0: fd8f fa1f f53f e8ff cbef ff33 b8f8 f0f6  .....?.....3....
+000000f0: e33e e67f e079 8fea 7fd7 7677 f4bf ab44  .>...y....vw...D
+00000100: c46a 73fe 1fa8 fe7f cf24 9d51 4907 3fb2  .js......$.QI.?.
+00000110: 52f0 3c3b 218e 691b 1f68 ca4e 881e 1bc6  R.<;!.i..h.N....
+00000120: 2642 0f12 e37a 95a6 b45c 37b1 e779 ca06  &B...z...\7..y..
+00000130: 055d 40f2 a594 8538 190e 175c 2e57 5333  .]@....8...\.WS3
+00000140: ced3 21a4 1924 fa00 494f 5772 9997 9051  ..!..$..IOWr...Q
+00000150: b764 1d1c b094 f2e4 8440 a6ef aa08 95d1  .d.......@......
+00000160: b862 ff5b f192 89c1 e51a 52c1 c5ff 15ba  .b.[......R.....
+00000170: a66d ddc9 df70 214f 485c ae0b 992f 4a5a  .m...p!OH\.../JZ
+00000180: 2cd7 a8ae feb6 fcef 045f f3bf 8bfc df0a  ,........_......
+00000190: ff3b f7f9 3f98 8c60 92e3 bc38 44fe bf3a  .;..?..`...8D..:
+000001a0: 3b7d f3fe cc4c 67fb e0ff e051 fe87 c59e  ;}...Lg....Q....
+000001b0: b7e1 7f30 0614 ff7b a311 f27f 1b78 45ae  ...0...{.....xE.
+000001c0: 59fc ee3d 49f8 b404 5a37 3e2d b968 02a4  Y..=I...Z7>-.h..
+000001d0: 28f3 1b3e 6382 c479 76c3 32ce 3249 681c  (..>c..yv.2.2Ih.
+000001e0: 3321 88cc 49c1 3342 3372 7dfd 8ec4 ac94  3!..I.3B3r}.....
+000001f0: 7cce 632a 998a a144 142c 5602 52ac a65f  |.c*...D.,V.R.._
+00000200: d8da 348c 57af c845 066d 9d24 5482 3961  ..4.W..E.m.$T.9a
+00000210: 7cfe fcd9 2878 4178 25ac cd09 2555 497f  |...(xAx%...%UI.
+00000220: 1060 5218 e7ac 6484 c27f 0156 0661 b734  .`R...d....V.a.4
+00000230: 2d12 a84d 3e27 2bc1 b305 e112 b293 199f  -..M>'+.........
+00000240: cf21 21d4 adaa 3767 c254 0515 da74 305e  .!!...7g.T...t0^
+00000250: d595 5993 5599 4085 6744 2ca9 e307 c6bc  ..Y.U.@.gD,.....
+00000260: ccd3 eab2 a610 09e1 6991 9712 4c0a 0677  ........i...L..w
+00000270: 1181 2482 bb96 ec56 1a5b e724 7c20 41af  ..$....V.[.$| A.
+00000280: d398 3e75 15cd aa54 3064 3ac7 a433 61c1  ..>u...T0d:..3a.
+00000290: c499 04d3 7930 1edb fed8 9d30 279e fbb1  ....y0.....0'...
+000002a0: eb78 ae3d 9ebb 9637 a563 3a9a 3167 ee8f  .x.=...7.c:.1g..
+000002b0: 478e e7c7 563c 1df9 73df 63ee 9cd9 93a0  G...V<..s.c.....
+000002c0: d387 26d1 d6d5 ad51 57b2 0ae8 bfe6 823d  ..&....QW......=
+000002d0: 5381 1b56 c2dd 875b 15d6 0552 9eab 5c4d  S..V...[...R..\M
+000002e0: 9154 acb3 98e7 9b60 1dab c564 c6e6 04ec  .T.....`...d....
+000002f0: b4ac d73f 3108 a092 fe06 865e 93d0 7c9d  ...?1......^..|.
+00000300: a8e1 710d 6303 7ab7 d787 24d0 b63a 5065  ..q.c.z...$..:Pe
+00000310: d9c9 56c7 3d5f 7ba8 f6bd aaab 82c1 002c  ..V.=_{........,
+00000320: f24c b0bb 9275 e9bf 5118 104d 9ca9 7ba6  .L...u..Q..M..{.
+00000330: 6fd4 f765 96ab ac57 dd82 befb bc60 19e5  o..e...W.....`..
+00000340: d518 a8ce 9b01 f011 42a7 17c7 e40d 9bd3  ........B.......
+00000350: 5522 cf55 2357 3767 c4fa 0063 a04a d3ab  U".U#W7g...c.J..
+00000360: daa2 e011 0cf1 b073 f6fe f2d3 cf9d 632d  .......s......c-
+00000370: 9c52 c122 186f e1e3 f736 bcb1 ebc4 2a49  .R.".o...6....*I
+00000380: 5495 1d7e 7dd5 de43 fdd7 37e2 2595 1056  T..~}..C..7.%..V
+00000390: 65aa f9a4 06a6 4e6e aa08 f32e 4298 d580  e.....Nn....B...
+000003a0: ad2a 9b42 b3c3 cc12 e12f 9ba6 fbe3 5e23  .*.B...../....^#
+000003b0: 76ca 3c61 9d13 d259 0956 d6f5 dbc4 e9cb  v.<a...Y.V......
+000003c0: 6752 455f d335 914a 57c0 3f4a 2413 722b  gRE_.5.JW.?J$.r+
+000003d0: f19f faec d74a 90e6 3306 ed90 c242 6300  .....J..3....Bc.
+000003e0: 933f a543 b5e6 18bc 53a7 0377 30fe f740  .?.C....S..w0..@
+000003f0: e985 7215 ab12 fa6a e222 2be3 fe1f eeff  ..r....j."+.....
+00000400: e1fe 1fa2 5dfb 5f9f 0ff7 33ff bfed f98f  ....]._...3.....
+00000410: eb3a 013e ffc1 fd1f d4ff edee ff58 93c0  .:.>.........X..
+00000420: 9be0 fecf 41eb ff28 e219 9751 6416 eb76  ....A..(...Qd..v
+00000430: f67f eef4 bf15 388e a3f6 7f7c cf75 70ff  ......8....|.up.
+00000440: 07ed 7fd4 ff68 ff23 dad5 ff42 24c3 979f  .....h.#...B$...
+00000450: ffdf 66ff c3df 11da ff68 ffa3 fe6f d7fe  ..f......h...o..
+00000460: b72d d7b6 d0fe 3f78 fdff b26b 8067 ed7f  .-....?x...k.g..
+00000470: 7f63 ffbb 9e07 bac0 0e1c 1fed ff56 a01f  .c...........V..
+00000480: 8099 cdd3 cdc7 9f81 e24c f967 02f9 1ff9  .........L.g....
+00000490: 7f8b ff5d cbc2 fd3f e4ff 5aeb bfd0 16e0  ...]...?..Z.....
+000004a0: 33fc 6f07 6e50 f3ff 08d2 d99a ff2d f4ff  3.o.nP.......-..
+000004b0: 6a8f ffb7 dda8 cd5b df9a 3486 4092 d359  j......[..4.@..Y
+000004c0: 54b0 3452 c268 cbcb cbf8 3adf 92fe 9e52  T.4R.h....:....R
+000004d0: 1832 254f b9e4 374c 3485 0856 729a f0df  .2%O..7L4..Vr...
+000004e0: 2bbf afc6 8389 8a65 c2a7 4d10 065d 55e4  +......e..M..]U.
+000004f0: aa4c 406c 16b4 14ac 2900 643a 6c18 8672  .L@l....).d:l..r
+00000500: 447a c001 0b52 28bf f2f2 b8f6 edd2 0112  Dz...R(.........
+00000510: 920f 79c6 6a97 a512 2a14 6e8a 5239 fa95  ..y.j...*.n.R9..
+00000520: f34d 2e94 470f 449b ea34 a329 d372 7de5  .M..G.D..4.).r}.
+00000530: 9078 9e4b f85c 4757 92aa 50c2 12a8 5f23  .x.K.\GW..P..._#
+00000540: d519 54eb a8b6 824c 5035 e5d8 14c1 9ddf  ..T....LP5......
+00000550: b072 bbdd 7a3d 7591 635d 7abf bfc9 0779  .r..z=u.c]z....y
+00000560: 1e6d ea5e 53b0 c9b2 389f b15e 7725 e783  .m.^S...8..^w%..
+00000570: 71b7 ce5e 39d8 45d3 b5d4 37a8 129b 204b  q..^9.E...7... K
+00000580: 78ac bc92 7afd 26a0 13f4 7411 3c5b 84f7  x...z.&...t.<[..
+00000590: 3ac5 3cab c5e6 9bb3 ab63 32cf 4be8 c99d  :.<......c2.K...
+000005a0: 2497 ba98 b73a cabc 5e4d ffcb 6259 c9be  $....:..^M..bY..
+000005b0: 67eb 8b6c 9edf ab4e d50d 509f ba9f cd4a  g..l...N..P....J
+000005c0: d0db ae6d df5c b2db 195f 30a1 fcb4 5466  ...m.\..._0...Tf
+000005d0: 68e8 3a23 1724 cba5 6eea 6df7 31a1 da6a  h.:#.$..n.m.1..j
+000005e0: e712 61e3 cfa7 1b73 e3a6 a7fa a01e 29b3  ..a....s......).
+000005f0: caa7 6a33 5a62 fdc6 43d8 b46b dfd8 2abc  ..j3Zb..C..k..*.
+00000600: d17c 3a52 c8bc 8481 26a9 14bd beba d21f  .|:R....&.......
+00000610: 5dd5 3bdd 1362 1f93 6e5c 2670 66c1 59d5  ].;..b..n\&pf.Y.
+00000620: 6554 85fe dcae 8659 b96e 45f3 842e 445d  eT.....Y.nE...D]
+00000630: a71f cfae 2ede fe1c fda4 b25c 9e5e 7dba  ...........\.^}.
+00000640: 387d 17bd 3e3f bdf8 508f 52b9 2a33 d29e  8}..>?..P.R.*3..
+00000650: d58d fbff b8ff 8ffb ff68 ff6d ec3f 932d  .........h.m.?.-
+00000660: 1603 0efa 7cf8 a2f3 ffdb f6ff 7d0b a271  ....|.......}..q
+00000670: ff1f d7ff a8ff db5d ff6b fd8f eb7f d4ff  .......].k......
+00000680: a0ff 5fec 75f0 6f7f ff3b b06d 0bd7 ff6d  .._.u.o..;.m...m
+00000690: 00df ff3e 6c20 ff23 ff23 ff23 ff3f c0ff  ...>l .#.#.#.?..
+000006a0: d71f 7fb8 7a7d 766d ca5b f902 fcff c4f3  ....z}vm.[......
+000006b0: 7fd7 1ded f2ff 08f7 ffdb c1e6 9d7f 4330  ..............C0
+000006c0: b92a cc62 6d7c e506 6e3c 6218 1a8f 0f98  .*.bm|..n<b.....
+000006d0: dda8 192b 5836 6359 bc8e 129e 7d11 0fa5  ...+X6cY....}...
+000006e0: 296b 6e7f 284e e645 94b0 1b96 dc45 ee3a  )kn.(N.E.....E.:
+000006f0: aa18 fb7a 7c85 fc8f fc8f fc8f 3834 fe7f  ...z|.......84..
+00000700: 4867 ef85 ff2d cbbe cfff 8e0d e991 ffdb  Hg...-..........
+00000710: 004e 75e4 7fe4 7fe4 7fe4 7fe4 ff27 d663  .Nu..........'.c
+00000720: 7b5d ff5b b6bf b3fe 1f79 b687 fcdf 0670  {].[.....y.....p
+00000730: 071d f91f f91f f91f f91f f9ff a93d d7bd  .............=..
+00000740: f2bf 15ec f2bf efe1 fabf bdfe c7f9 8efc  ................
+00000750: 8ffe df87 c9ff e8ff 8dfc bfe1 7ff5 0438  ...............8
+00000760: 9e2f f630 ff9f e47f 6f97 ff3d cbc3 f57f  ./.0....o..=....
+00000770: 2bf8 05cc bd48 997b bf1a 922e a2e9 8a27  +....H.{.......'
+00000780: 3312 121d 98a9 9f73 0f89 65a0 2640 fec7  3......s..e.&@..
+00000790: f5ff 21ac ff2d 6fec e3fa ffa0 f9ff e59d  ..!..-o.........
+000007a0: a69e e37f df72 36bf ff33 727c f5fb cf23  .....r6..3r|...#
+000007b0: df46 fe6f 03f5 4750 a0e3 659e 275b efec  .F.o..GP..e.'[..
+000007c0: 83c4 a87c 02ab 2f47 a817 e3c3 ae1e 2edd  ...|../G........
+000007d0: eac3 0e37 d58b 0161 578f 9e5a 3863 222e  ...7...aW..Z8c".
+000007e0: 7921 75c4 766a aadd fd41 a6db f19e 30d2  y!u.vj...A....0.
+000007f0: ef00 84dd fbef 00d4 49d4 4734 bacf bc5a  ........I.G4...Z
+00000800: 5027 2d68 fca5 fab8 4573 65d2 dd7c dfa5  P'-h....Ese..|..
+00000810: 5b7f 8ea2 fede 4cd4 3cdd dafa 1246 77fb  [.....L.<....Fw.
+00000820: 6148 77fb 1b16 d5a7 64ee f274 abd7 11ba  aHw.....d..t....
+00000830: ea83 15a8 4310 0804 0281 4020 1008 0402  ....C.....@ ....
+00000840: 8140 2010 0804 0281 4020 1008 0402 8140  .@ .....@ .....@
+00000850: 2010 08c4 ff07 7f01 eec8 574f 00a0 0000   .........WO....
```


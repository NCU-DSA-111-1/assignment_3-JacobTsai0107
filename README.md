# __Assignment 4 : Arithmetic Coding VS Huffman Coding__
## Introduction

## Compile & Run 

```sh
# Compile
cd ~/桌面/hw4/arithmetic_coding(huffman_coding) 
//路徑位置不一定相同，可依自身路徑調整
##for arithmetic
gcc -o arcd arcd_stream.c arcd.c arcd.h adaptive_model.h adaptive_model.c 
##for huffman
gcc -o huffman huffcode.c huffman.c huffman.h 
ls
# Run
##for arithmetic
./arcd -e <testfilename | tee encodingtext
./arcd -d <encodingtext | tee decodingtext
##for huffman
./huffman -i testfilename -o encodingtext -c
./huffman -i encodingtext -o decodingtext -d
```
## Usage
```c
//take testessay for example
//for arithmetic encoding
LCc6�f<�Оǝñ�ǖ��rp�      ���7���=���c�����Em,�܂ ��G[M�w���M��c$�Q5V\�1�I͸}�[W͡���+<%J��&u����8y�� � (�_��]�g/�Y��)ڪ�ʃ�E*ٍ��:�ɒ���z�1��`7��-.���fED�^��۹ȩ39T�����)/�ѯ�H��{'3�OB�iBX�뷙��2b��M����g�m��쎳�W&ӟ
                                                                               ���O�m�4W\ޘ��P5�+k��|}�K��̤G�Ԯ�c��\���q�� o
�)vMH�g���V[�1F�?a��-�G�*��t��J��"/�I�3$z��SF��
                                               z@��,]�g��W�M>��o�'���F���a������A�VWG�uCI�=���bb�Ԓ����>E?ۢ��5
                                                                                                            KZ�sD��v��J���
 ���5��
s�={�Ȼ;�$�p��l�$��홥OR4��
.�bF�r>���7��H�?�i���8�{�v��D�Y�}@�3���r�ΰ�ҙQd�s0։�|H'Ķo`Z&��&�!O�D�,���?�
                                                                          ���h
the coding time is 0.000509 sec.
//for arithmetic decoding
Let us not wallow in the valley of despair, I say to you today, my friends.

And so even though we face the difficulties of today and tomorrow, I still have a dream. It is a dream deeply rooted in the American dream.

I have a dream that one day this nation will rise up and live out the true meaning of its creed: "We hold these truths to be self-evident, that all men are created equal."

I have a dream that one day on the red hills of Georgia, the sons of former slaves and the sons of former slave owners will be able to sit down together at the table of brotherhood.

I have a dream that one day even the state of Mississippi, a state sweltering with the heat of injustice, sweltering with the heat of oppression, will be transformed into an oasis of freedom and justice.

I have a dream that my four little children will one day live in a nation where they will not be judged by the color of their skin but by the content of their character.

I have a dream today!

the coding time is 0.000733 sec.
//for huffman encoding
the coding time is 0.000103 sec.
//for huffman decoding
the coding time is 0.000080 sec.
```
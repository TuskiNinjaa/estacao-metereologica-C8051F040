                                      1 ;--------------------------------------------------------
                                      2 ; File Created by SDCC : free open source ANSI-C Compiler
                                      3 ; Version 3.6.0 #9615 (MINGW64)
                                      4 ;--------------------------------------------------------
                                      5 	.module main
                                      6 	.optsdcc -mmcs51 --model-small
                                      7 	
                                      8 ;--------------------------------------------------------
                                      9 ; Public variables in this module
                                     10 ;--------------------------------------------------------
                                     11 	.globl _ini_relogio_PARM_6
                                     12 	.globl _ini_relogio_PARM_5
                                     13 	.globl _ini_relogio_PARM_4
                                     14 	.globl _ini_relogio_PARM_3
                                     15 	.globl _ini_relogio_PARM_2
                                     16 	.globl _esc_RAM_SPI_PARM_2
                                     17 	.globl _le_adc0_PARM_4
                                     18 	.globl _le_adc0_PARM_3
                                     19 	.globl _le_adc0_PARM_2
                                     20 	.globl _fonte
                                     21 	.globl _main
                                     22 	.globl _executa_comando
                                     23 	.globl _imprime_terminal_tempo_real
                                     24 	.globl _imprime_glcd_tempo_real
                                     25 	.globl _ligar_buzzer
                                     26 	.globl _isr_UART0
                                     27 	.globl _isr_tempo
                                     28 	.globl _demonstra_amostras
                                     29 	.globl _coleta_amostra
                                     30 	.globl _ini_relogio
                                     31 	.globl _ano_bissexto
                                     32 	.globl _print_relogio_glcd
                                     33 	.globl _print_relogio_terminal
                                     34 	.globl _verifica_RAM_SPI
                                     35 	.globl _le_RAM_SPI
                                     36 	.globl _esc_RAM_SPI
                                     37 	.globl _le_sensores
                                     38 	.globl _le_voltagem
                                     39 	.globl _le_adc0
                                     40 	.globl _le_dht11
                                     41 	.globl _le_byte_dht11
                                     42 	.globl _resposta_dht11
                                     43 	.globl _inicia_dht11
                                     44 	.globl _delay_us
                                     45 	.globl _delay_ms
                                     46 	.globl _escreve_caractere
                                     47 	.globl _caractere_para_ascii
                                     48 	.globl _limpa_glcd
                                     49 	.globl _conf_pag
                                     50 	.globl _conf_Y
                                     51 	.globl _ini_glcd
                                     52 	.globl _esc_glcd
                                     53 	.globl _le_glcd
                                     54 	.globl _Init_Device
                                     55 	.globl _Interrupts_Init
                                     56 	.globl _Oscillator_Init
                                     57 	.globl _Port_IO_Init
                                     58 	.globl _Voltage_Reference_Init
                                     59 	.globl _DAC_Init
                                     60 	.globl _ADC_Init
                                     61 	.globl _SPI_Init
                                     62 	.globl _SMBus_Init
                                     63 	.globl _UART_Init
                                     64 	.globl _Timer_Init
                                     65 	.globl _Reset_Sources_Init
                                     66 	.globl _printf_fast_f
                                     67 	.globl _P7_7
                                     68 	.globl _P7_6
                                     69 	.globl _P7_5
                                     70 	.globl _P7_4
                                     71 	.globl _P7_3
                                     72 	.globl _P7_2
                                     73 	.globl _P7_1
                                     74 	.globl _P7_0
                                     75 	.globl _P6_7
                                     76 	.globl _P6_6
                                     77 	.globl _P6_5
                                     78 	.globl _P6_4
                                     79 	.globl _P6_3
                                     80 	.globl _P6_2
                                     81 	.globl _P6_1
                                     82 	.globl _P6_0
                                     83 	.globl _P5_7
                                     84 	.globl _P5_6
                                     85 	.globl _P5_5
                                     86 	.globl _P5_4
                                     87 	.globl _P5_3
                                     88 	.globl _P5_2
                                     89 	.globl _P5_1
                                     90 	.globl _P5_0
                                     91 	.globl _P4_7
                                     92 	.globl _P4_6
                                     93 	.globl _P4_5
                                     94 	.globl _P4_4
                                     95 	.globl _P4_3
                                     96 	.globl _P4_2
                                     97 	.globl _P4_1
                                     98 	.globl _P4_0
                                     99 	.globl _P3_7
                                    100 	.globl _P3_6
                                    101 	.globl _P3_5
                                    102 	.globl _P3_4
                                    103 	.globl _P3_3
                                    104 	.globl _P3_2
                                    105 	.globl _P3_1
                                    106 	.globl _P3_0
                                    107 	.globl _P2_7
                                    108 	.globl _P2_6
                                    109 	.globl _P2_5
                                    110 	.globl _P2_4
                                    111 	.globl _P2_3
                                    112 	.globl _P2_2
                                    113 	.globl _P2_1
                                    114 	.globl _P2_0
                                    115 	.globl _P1_7
                                    116 	.globl _P1_6
                                    117 	.globl _P1_5
                                    118 	.globl _P1_4
                                    119 	.globl _P1_3
                                    120 	.globl _P1_2
                                    121 	.globl _P1_1
                                    122 	.globl _P1_0
                                    123 	.globl _P0_7
                                    124 	.globl _P0_6
                                    125 	.globl _P0_5
                                    126 	.globl _P0_4
                                    127 	.globl _P0_3
                                    128 	.globl _P0_2
                                    129 	.globl _P0_1
                                    130 	.globl _P0_0
                                    131 	.globl _CANTEST
                                    132 	.globl _CANCCE
                                    133 	.globl _CANDAR
                                    134 	.globl _CANIF
                                    135 	.globl _CANEIE
                                    136 	.globl _CANSIE
                                    137 	.globl _CANIE
                                    138 	.globl _CANINIT
                                    139 	.globl _SPIEN
                                    140 	.globl _TXBMT
                                    141 	.globl _NSSMD0
                                    142 	.globl _NSSMD1
                                    143 	.globl _RXOVRN
                                    144 	.globl _MODF
                                    145 	.globl _WCOL
                                    146 	.globl _SPIF
                                    147 	.globl _AD2WINT
                                    148 	.globl _AD2CM0
                                    149 	.globl _AD2CM1
                                    150 	.globl _AD2CM2
                                    151 	.globl _AD2BUSY
                                    152 	.globl _AD2INT
                                    153 	.globl _AD2TM
                                    154 	.globl _AD2EN
                                    155 	.globl _AD0LJST
                                    156 	.globl _AD0WINT
                                    157 	.globl _AD0CM0
                                    158 	.globl _AD0CM1
                                    159 	.globl _AD0BUSY
                                    160 	.globl _AD0INT
                                    161 	.globl _AD0TM
                                    162 	.globl _AD0EN
                                    163 	.globl _CCF0
                                    164 	.globl _CCF1
                                    165 	.globl _CCF2
                                    166 	.globl _CCF3
                                    167 	.globl _CCF4
                                    168 	.globl _CCF5
                                    169 	.globl _CR
                                    170 	.globl _CF
                                    171 	.globl _P
                                    172 	.globl _F1
                                    173 	.globl _OV
                                    174 	.globl _RS0
                                    175 	.globl _RS1
                                    176 	.globl _F0
                                    177 	.globl _AC
                                    178 	.globl _CY
                                    179 	.globl _CPRL4
                                    180 	.globl _CT4
                                    181 	.globl _TR4
                                    182 	.globl _EXEN4
                                    183 	.globl _EXF4
                                    184 	.globl _TF4
                                    185 	.globl _CPRL3
                                    186 	.globl _CT3
                                    187 	.globl _TR3
                                    188 	.globl _EXEN3
                                    189 	.globl _EXF3
                                    190 	.globl _TF3
                                    191 	.globl _CPRL2
                                    192 	.globl _CT2
                                    193 	.globl _TR2
                                    194 	.globl _EXEN2
                                    195 	.globl _EXF2
                                    196 	.globl _TF2
                                    197 	.globl _LEC0
                                    198 	.globl _LEC1
                                    199 	.globl _LEC2
                                    200 	.globl _TXOK
                                    201 	.globl _RXOK
                                    202 	.globl _EPASS
                                    203 	.globl _EWARN
                                    204 	.globl _BOFF
                                    205 	.globl _SMBTOE
                                    206 	.globl _SMBFTE
                                    207 	.globl _AA
                                    208 	.globl _SI
                                    209 	.globl _STO
                                    210 	.globl _STA
                                    211 	.globl _ENSMB
                                    212 	.globl _BUSY
                                    213 	.globl _PX0
                                    214 	.globl _PT0
                                    215 	.globl _PX1
                                    216 	.globl _PT1
                                    217 	.globl _PS0
                                    218 	.globl _PT2
                                    219 	.globl _EX0
                                    220 	.globl _ET0
                                    221 	.globl _EX1
                                    222 	.globl _ET1
                                    223 	.globl _ES0
                                    224 	.globl _ET2
                                    225 	.globl _EA
                                    226 	.globl _RI1
                                    227 	.globl _TI1
                                    228 	.globl _RB81
                                    229 	.globl _TB81
                                    230 	.globl _REN1
                                    231 	.globl _MCE1
                                    232 	.globl _S1MODE
                                    233 	.globl _RI0
                                    234 	.globl _TI0
                                    235 	.globl _RB80
                                    236 	.globl _TB80
                                    237 	.globl _REN0
                                    238 	.globl _SM20
                                    239 	.globl _SM10
                                    240 	.globl _SM00
                                    241 	.globl _CP2HYN0
                                    242 	.globl _CP2HYN1
                                    243 	.globl _CP2HYP0
                                    244 	.globl _CP2HYP1
                                    245 	.globl _CP2FIF
                                    246 	.globl _CP2RIF
                                    247 	.globl _CP2OUT
                                    248 	.globl _CP2EN
                                    249 	.globl _CP1HYN0
                                    250 	.globl _CP1HYN1
                                    251 	.globl _CP1HYP0
                                    252 	.globl _CP1HYP1
                                    253 	.globl _CP1FIF
                                    254 	.globl _CP1RIF
                                    255 	.globl _CP1OUT
                                    256 	.globl _CP1EN
                                    257 	.globl _CP0HYN0
                                    258 	.globl _CP0HYN1
                                    259 	.globl _CP0HYP0
                                    260 	.globl _CP0HYP1
                                    261 	.globl _CP0FIF
                                    262 	.globl _CP0RIF
                                    263 	.globl _CP0OUT
                                    264 	.globl _CP0EN
                                    265 	.globl _IT0
                                    266 	.globl _IE0
                                    267 	.globl _IT1
                                    268 	.globl _IE1
                                    269 	.globl _TR0
                                    270 	.globl _TF0
                                    271 	.globl _TR1
                                    272 	.globl _TF1
                                    273 	.globl __XPAGE
                                    274 	.globl _DP
                                    275 	.globl _ADC0
                                    276 	.globl _ADC0LT
                                    277 	.globl _ADC0GT
                                    278 	.globl _TMR4
                                    279 	.globl _TMR3
                                    280 	.globl _TMR2
                                    281 	.globl _RCAP4
                                    282 	.globl _RCAP3
                                    283 	.globl _RCAP2
                                    284 	.globl _DAC1
                                    285 	.globl _DAC0
                                    286 	.globl _CAN0DAT
                                    287 	.globl _PCA0CP5
                                    288 	.globl _PCA0CP4
                                    289 	.globl _PCA0CP3
                                    290 	.globl _PCA0CP2
                                    291 	.globl _PCA0CP1
                                    292 	.globl _PCA0CP0
                                    293 	.globl _PCA0
                                    294 	.globl _WDTCN
                                    295 	.globl _PCA0CPH1
                                    296 	.globl _PCA0CPL1
                                    297 	.globl _PCA0CPH0
                                    298 	.globl _PCA0CPL0
                                    299 	.globl _PCA0H
                                    300 	.globl _PCA0L
                                    301 	.globl _P7
                                    302 	.globl _CAN0CN
                                    303 	.globl _SPI0CN
                                    304 	.globl _EIP2
                                    305 	.globl _EIP1
                                    306 	.globl _B
                                    307 	.globl _RSTSRC
                                    308 	.globl _PCA0CPH4
                                    309 	.globl _PCA0CPL4
                                    310 	.globl _PCA0CPH3
                                    311 	.globl _PCA0CPL3
                                    312 	.globl _PCA0CPH2
                                    313 	.globl _PCA0CPL2
                                    314 	.globl _P6
                                    315 	.globl _ADC2CN
                                    316 	.globl _ADC0CN
                                    317 	.globl _EIE2
                                    318 	.globl _EIE1
                                    319 	.globl _XBR3
                                    320 	.globl _XBR2
                                    321 	.globl _XBR1
                                    322 	.globl _PCA0CPH5
                                    323 	.globl _XBR0
                                    324 	.globl _PCA0CPL5
                                    325 	.globl _ACC
                                    326 	.globl _PCA0CPM5
                                    327 	.globl _PCA0CPM4
                                    328 	.globl _PCA0CPM3
                                    329 	.globl _PCA0CPM2
                                    330 	.globl _CAN0TST
                                    331 	.globl _PCA0CPM1
                                    332 	.globl _CAN0ADR
                                    333 	.globl _PCA0CPM0
                                    334 	.globl _CAN0DATH
                                    335 	.globl _PCA0MD
                                    336 	.globl _P5
                                    337 	.globl _CAN0DATL
                                    338 	.globl _PCA0CN
                                    339 	.globl _HVA0CN
                                    340 	.globl _DAC1CN
                                    341 	.globl _DAC0CN
                                    342 	.globl _DAC1H
                                    343 	.globl _DAC0H
                                    344 	.globl _DAC1L
                                    345 	.globl _DAC0L
                                    346 	.globl _REF0CN
                                    347 	.globl _PSW
                                    348 	.globl _SMB0CR
                                    349 	.globl _TMR4H
                                    350 	.globl _TMR3H
                                    351 	.globl _TMR2H
                                    352 	.globl _TMR4L
                                    353 	.globl _TMR3L
                                    354 	.globl _TMR2L
                                    355 	.globl _RCAP4H
                                    356 	.globl _RCAP3H
                                    357 	.globl _RCAP2H
                                    358 	.globl _RCAP4L
                                    359 	.globl _RCAP3L
                                    360 	.globl _RCAP2L
                                    361 	.globl _TMR4CF
                                    362 	.globl _TMR3CF
                                    363 	.globl _TMR2CF
                                    364 	.globl _P4
                                    365 	.globl _TMR4CN
                                    366 	.globl _TMR3CN
                                    367 	.globl _TMR2CN
                                    368 	.globl _ADC0LTH
                                    369 	.globl _ADC2LT
                                    370 	.globl _ADC0LTL
                                    371 	.globl _ADC0GTH
                                    372 	.globl _ADC2GT
                                    373 	.globl _ADC0GTL
                                    374 	.globl _SMB0ADR
                                    375 	.globl _SMB0DAT
                                    376 	.globl _SMB0STA
                                    377 	.globl _CAN0STA
                                    378 	.globl _SMB0CN
                                    379 	.globl _ADC0H
                                    380 	.globl _ADC2
                                    381 	.globl _ADC0L
                                    382 	.globl _ADC2CF
                                    383 	.globl _ADC0CF
                                    384 	.globl _AMX2SL
                                    385 	.globl _AMX0SL
                                    386 	.globl _AMX0CF
                                    387 	.globl _AMX0PRT
                                    388 	.globl _AMX2CF
                                    389 	.globl _SADEN0
                                    390 	.globl _IP
                                    391 	.globl _FLACL
                                    392 	.globl _FLSCL
                                    393 	.globl _P3
                                    394 	.globl _P3MDIN
                                    395 	.globl _P2MDIN
                                    396 	.globl _P1MDIN
                                    397 	.globl _SADDR1
                                    398 	.globl _SADDR0
                                    399 	.globl _IE
                                    400 	.globl _P3MDOUT
                                    401 	.globl _P2MDOUT
                                    402 	.globl _P1MDOUT
                                    403 	.globl _P0MDOUT
                                    404 	.globl _EMI0CF
                                    405 	.globl _EMI0CN
                                    406 	.globl _EMI0TC
                                    407 	.globl _P2
                                    408 	.globl _P7MDOUT
                                    409 	.globl _P6MDOUT
                                    410 	.globl _P5MDOUT
                                    411 	.globl _SPI0CKR
                                    412 	.globl _P4MDOUT
                                    413 	.globl _SPI0DAT
                                    414 	.globl _SPI0CFG
                                    415 	.globl _SBUF1
                                    416 	.globl _SBUF0
                                    417 	.globl _SCON1
                                    418 	.globl _SCON0
                                    419 	.globl _CLKSEL
                                    420 	.globl _SFRPGCN
                                    421 	.globl _SSTA0
                                    422 	.globl _P1
                                    423 	.globl _PSCTL
                                    424 	.globl _CKCON
                                    425 	.globl _TH1
                                    426 	.globl _OSCXCN
                                    427 	.globl _TH0
                                    428 	.globl _OSCICL
                                    429 	.globl _TL1
                                    430 	.globl _OSCICN
                                    431 	.globl _TL0
                                    432 	.globl _CPT2MD
                                    433 	.globl _CPT1MD
                                    434 	.globl _CPT0MD
                                    435 	.globl _TMOD
                                    436 	.globl _CPT2CN
                                    437 	.globl _CPT1CN
                                    438 	.globl _CPT0CN
                                    439 	.globl _TCON
                                    440 	.globl _PCON
                                    441 	.globl _SFRLAST
                                    442 	.globl _SFRNEXT
                                    443 	.globl _SFRPAGE
                                    444 	.globl _DPH
                                    445 	.globl _DPL
                                    446 	.globl _SP
                                    447 	.globl _P0
                                    448 	.globl _flag_tecla
                                    449 	.globl _transmissao_dht11
                                    450 	.globl _escreve_caractere_PARM_2
                                    451 	.globl _limpa_glcd_PARM_1
                                    452 	.globl _conf_pag_PARM_2
                                    453 	.globl _conf_Y_PARM_2
                                    454 	.globl _esc_glcd_PARM_3
                                    455 	.globl _esc_glcd_PARM_2
                                    456 	.globl _le_glcd_PARM_2
                                    457 	.globl _le_glcd_PARM_1
                                    458 	.globl _terminal_ativo
                                    459 	.globl _ligar_buzzer_PARM_2
                                    460 	.globl _tecla
                                    461 	.globl _relogio
                                    462 	.globl _end_fim_ram
                                    463 	.globl _le_voltagem_PARM_2
                                    464 	.globl _saida
                                    465 	.globl _conta_caractere
                                    466 	.globl _putchar
                                    467 ;--------------------------------------------------------
                                    468 ; special function registers
                                    469 ;--------------------------------------------------------
                                    470 	.area RSEG    (ABS,DATA)
      000000                        471 	.org 0x0000
                           000080   472 G$P0$0$0 == 0x0080
                           000080   473 _P0	=	0x0080
                           000081   474 G$SP$0$0 == 0x0081
                           000081   475 _SP	=	0x0081
                           000082   476 G$DPL$0$0 == 0x0082
                           000082   477 _DPL	=	0x0082
                           000083   478 G$DPH$0$0 == 0x0083
                           000083   479 _DPH	=	0x0083
                           000084   480 G$SFRPAGE$0$0 == 0x0084
                           000084   481 _SFRPAGE	=	0x0084
                           000085   482 G$SFRNEXT$0$0 == 0x0085
                           000085   483 _SFRNEXT	=	0x0085
                           000086   484 G$SFRLAST$0$0 == 0x0086
                           000086   485 _SFRLAST	=	0x0086
                           000087   486 G$PCON$0$0 == 0x0087
                           000087   487 _PCON	=	0x0087
                           000088   488 G$TCON$0$0 == 0x0088
                           000088   489 _TCON	=	0x0088
                           000088   490 G$CPT0CN$0$0 == 0x0088
                           000088   491 _CPT0CN	=	0x0088
                           000088   492 G$CPT1CN$0$0 == 0x0088
                           000088   493 _CPT1CN	=	0x0088
                           000088   494 G$CPT2CN$0$0 == 0x0088
                           000088   495 _CPT2CN	=	0x0088
                           000089   496 G$TMOD$0$0 == 0x0089
                           000089   497 _TMOD	=	0x0089
                           000089   498 G$CPT0MD$0$0 == 0x0089
                           000089   499 _CPT0MD	=	0x0089
                           000089   500 G$CPT1MD$0$0 == 0x0089
                           000089   501 _CPT1MD	=	0x0089
                           000089   502 G$CPT2MD$0$0 == 0x0089
                           000089   503 _CPT2MD	=	0x0089
                           00008A   504 G$TL0$0$0 == 0x008a
                           00008A   505 _TL0	=	0x008a
                           00008A   506 G$OSCICN$0$0 == 0x008a
                           00008A   507 _OSCICN	=	0x008a
                           00008B   508 G$TL1$0$0 == 0x008b
                           00008B   509 _TL1	=	0x008b
                           00008B   510 G$OSCICL$0$0 == 0x008b
                           00008B   511 _OSCICL	=	0x008b
                           00008C   512 G$TH0$0$0 == 0x008c
                           00008C   513 _TH0	=	0x008c
                           00008C   514 G$OSCXCN$0$0 == 0x008c
                           00008C   515 _OSCXCN	=	0x008c
                           00008D   516 G$TH1$0$0 == 0x008d
                           00008D   517 _TH1	=	0x008d
                           00008E   518 G$CKCON$0$0 == 0x008e
                           00008E   519 _CKCON	=	0x008e
                           00008F   520 G$PSCTL$0$0 == 0x008f
                           00008F   521 _PSCTL	=	0x008f
                           000090   522 G$P1$0$0 == 0x0090
                           000090   523 _P1	=	0x0090
                           000091   524 G$SSTA0$0$0 == 0x0091
                           000091   525 _SSTA0	=	0x0091
                           000096   526 G$SFRPGCN$0$0 == 0x0096
                           000096   527 _SFRPGCN	=	0x0096
                           000097   528 G$CLKSEL$0$0 == 0x0097
                           000097   529 _CLKSEL	=	0x0097
                           000098   530 G$SCON0$0$0 == 0x0098
                           000098   531 _SCON0	=	0x0098
                           000098   532 G$SCON1$0$0 == 0x0098
                           000098   533 _SCON1	=	0x0098
                           000099   534 G$SBUF0$0$0 == 0x0099
                           000099   535 _SBUF0	=	0x0099
                           000099   536 G$SBUF1$0$0 == 0x0099
                           000099   537 _SBUF1	=	0x0099
                           00009A   538 G$SPI0CFG$0$0 == 0x009a
                           00009A   539 _SPI0CFG	=	0x009a
                           00009B   540 G$SPI0DAT$0$0 == 0x009b
                           00009B   541 _SPI0DAT	=	0x009b
                           00009C   542 G$P4MDOUT$0$0 == 0x009c
                           00009C   543 _P4MDOUT	=	0x009c
                           00009D   544 G$SPI0CKR$0$0 == 0x009d
                           00009D   545 _SPI0CKR	=	0x009d
                           00009D   546 G$P5MDOUT$0$0 == 0x009d
                           00009D   547 _P5MDOUT	=	0x009d
                           00009E   548 G$P6MDOUT$0$0 == 0x009e
                           00009E   549 _P6MDOUT	=	0x009e
                           00009F   550 G$P7MDOUT$0$0 == 0x009f
                           00009F   551 _P7MDOUT	=	0x009f
                           0000A0   552 G$P2$0$0 == 0x00a0
                           0000A0   553 _P2	=	0x00a0
                           0000A1   554 G$EMI0TC$0$0 == 0x00a1
                           0000A1   555 _EMI0TC	=	0x00a1
                           0000A2   556 G$EMI0CN$0$0 == 0x00a2
                           0000A2   557 _EMI0CN	=	0x00a2
                           0000A3   558 G$EMI0CF$0$0 == 0x00a3
                           0000A3   559 _EMI0CF	=	0x00a3
                           0000A4   560 G$P0MDOUT$0$0 == 0x00a4
                           0000A4   561 _P0MDOUT	=	0x00a4
                           0000A5   562 G$P1MDOUT$0$0 == 0x00a5
                           0000A5   563 _P1MDOUT	=	0x00a5
                           0000A6   564 G$P2MDOUT$0$0 == 0x00a6
                           0000A6   565 _P2MDOUT	=	0x00a6
                           0000A7   566 G$P3MDOUT$0$0 == 0x00a7
                           0000A7   567 _P3MDOUT	=	0x00a7
                           0000A8   568 G$IE$0$0 == 0x00a8
                           0000A8   569 _IE	=	0x00a8
                           0000A9   570 G$SADDR0$0$0 == 0x00a9
                           0000A9   571 _SADDR0	=	0x00a9
                           0000A9   572 G$SADDR1$0$0 == 0x00a9
                           0000A9   573 _SADDR1	=	0x00a9
                           0000AD   574 G$P1MDIN$0$0 == 0x00ad
                           0000AD   575 _P1MDIN	=	0x00ad
                           0000AE   576 G$P2MDIN$0$0 == 0x00ae
                           0000AE   577 _P2MDIN	=	0x00ae
                           0000AF   578 G$P3MDIN$0$0 == 0x00af
                           0000AF   579 _P3MDIN	=	0x00af
                           0000B0   580 G$P3$0$0 == 0x00b0
                           0000B0   581 _P3	=	0x00b0
                           0000B7   582 G$FLSCL$0$0 == 0x00b7
                           0000B7   583 _FLSCL	=	0x00b7
                           0000B7   584 G$FLACL$0$0 == 0x00b7
                           0000B7   585 _FLACL	=	0x00b7
                           0000B8   586 G$IP$0$0 == 0x00b8
                           0000B8   587 _IP	=	0x00b8
                           0000B9   588 G$SADEN0$0$0 == 0x00b9
                           0000B9   589 _SADEN0	=	0x00b9
                           0000BA   590 G$AMX2CF$0$0 == 0x00ba
                           0000BA   591 _AMX2CF	=	0x00ba
                           0000BD   592 G$AMX0PRT$0$0 == 0x00bd
                           0000BD   593 _AMX0PRT	=	0x00bd
                           0000BA   594 G$AMX0CF$0$0 == 0x00ba
                           0000BA   595 _AMX0CF	=	0x00ba
                           0000BB   596 G$AMX0SL$0$0 == 0x00bb
                           0000BB   597 _AMX0SL	=	0x00bb
                           0000BB   598 G$AMX2SL$0$0 == 0x00bb
                           0000BB   599 _AMX2SL	=	0x00bb
                           0000BC   600 G$ADC0CF$0$0 == 0x00bc
                           0000BC   601 _ADC0CF	=	0x00bc
                           0000BC   602 G$ADC2CF$0$0 == 0x00bc
                           0000BC   603 _ADC2CF	=	0x00bc
                           0000BE   604 G$ADC0L$0$0 == 0x00be
                           0000BE   605 _ADC0L	=	0x00be
                           0000BE   606 G$ADC2$0$0 == 0x00be
                           0000BE   607 _ADC2	=	0x00be
                           0000BF   608 G$ADC0H$0$0 == 0x00bf
                           0000BF   609 _ADC0H	=	0x00bf
                           0000C0   610 G$SMB0CN$0$0 == 0x00c0
                           0000C0   611 _SMB0CN	=	0x00c0
                           0000C0   612 G$CAN0STA$0$0 == 0x00c0
                           0000C0   613 _CAN0STA	=	0x00c0
                           0000C1   614 G$SMB0STA$0$0 == 0x00c1
                           0000C1   615 _SMB0STA	=	0x00c1
                           0000C2   616 G$SMB0DAT$0$0 == 0x00c2
                           0000C2   617 _SMB0DAT	=	0x00c2
                           0000C3   618 G$SMB0ADR$0$0 == 0x00c3
                           0000C3   619 _SMB0ADR	=	0x00c3
                           0000C4   620 G$ADC0GTL$0$0 == 0x00c4
                           0000C4   621 _ADC0GTL	=	0x00c4
                           0000C4   622 G$ADC2GT$0$0 == 0x00c4
                           0000C4   623 _ADC2GT	=	0x00c4
                           0000C5   624 G$ADC0GTH$0$0 == 0x00c5
                           0000C5   625 _ADC0GTH	=	0x00c5
                           0000C6   626 G$ADC0LTL$0$0 == 0x00c6
                           0000C6   627 _ADC0LTL	=	0x00c6
                           0000C6   628 G$ADC2LT$0$0 == 0x00c6
                           0000C6   629 _ADC2LT	=	0x00c6
                           0000C7   630 G$ADC0LTH$0$0 == 0x00c7
                           0000C7   631 _ADC0LTH	=	0x00c7
                           0000C8   632 G$TMR2CN$0$0 == 0x00c8
                           0000C8   633 _TMR2CN	=	0x00c8
                           0000C8   634 G$TMR3CN$0$0 == 0x00c8
                           0000C8   635 _TMR3CN	=	0x00c8
                           0000C8   636 G$TMR4CN$0$0 == 0x00c8
                           0000C8   637 _TMR4CN	=	0x00c8
                           0000C8   638 G$P4$0$0 == 0x00c8
                           0000C8   639 _P4	=	0x00c8
                           0000C9   640 G$TMR2CF$0$0 == 0x00c9
                           0000C9   641 _TMR2CF	=	0x00c9
                           0000C9   642 G$TMR3CF$0$0 == 0x00c9
                           0000C9   643 _TMR3CF	=	0x00c9
                           0000C9   644 G$TMR4CF$0$0 == 0x00c9
                           0000C9   645 _TMR4CF	=	0x00c9
                           0000CA   646 G$RCAP2L$0$0 == 0x00ca
                           0000CA   647 _RCAP2L	=	0x00ca
                           0000CA   648 G$RCAP3L$0$0 == 0x00ca
                           0000CA   649 _RCAP3L	=	0x00ca
                           0000CA   650 G$RCAP4L$0$0 == 0x00ca
                           0000CA   651 _RCAP4L	=	0x00ca
                           0000CB   652 G$RCAP2H$0$0 == 0x00cb
                           0000CB   653 _RCAP2H	=	0x00cb
                           0000CB   654 G$RCAP3H$0$0 == 0x00cb
                           0000CB   655 _RCAP3H	=	0x00cb
                           0000CB   656 G$RCAP4H$0$0 == 0x00cb
                           0000CB   657 _RCAP4H	=	0x00cb
                           0000CC   658 G$TMR2L$0$0 == 0x00cc
                           0000CC   659 _TMR2L	=	0x00cc
                           0000CC   660 G$TMR3L$0$0 == 0x00cc
                           0000CC   661 _TMR3L	=	0x00cc
                           0000CC   662 G$TMR4L$0$0 == 0x00cc
                           0000CC   663 _TMR4L	=	0x00cc
                           0000CD   664 G$TMR2H$0$0 == 0x00cd
                           0000CD   665 _TMR2H	=	0x00cd
                           0000CD   666 G$TMR3H$0$0 == 0x00cd
                           0000CD   667 _TMR3H	=	0x00cd
                           0000CD   668 G$TMR4H$0$0 == 0x00cd
                           0000CD   669 _TMR4H	=	0x00cd
                           0000CF   670 G$SMB0CR$0$0 == 0x00cf
                           0000CF   671 _SMB0CR	=	0x00cf
                           0000D0   672 G$PSW$0$0 == 0x00d0
                           0000D0   673 _PSW	=	0x00d0
                           0000D1   674 G$REF0CN$0$0 == 0x00d1
                           0000D1   675 _REF0CN	=	0x00d1
                           0000D2   676 G$DAC0L$0$0 == 0x00d2
                           0000D2   677 _DAC0L	=	0x00d2
                           0000D2   678 G$DAC1L$0$0 == 0x00d2
                           0000D2   679 _DAC1L	=	0x00d2
                           0000D3   680 G$DAC0H$0$0 == 0x00d3
                           0000D3   681 _DAC0H	=	0x00d3
                           0000D3   682 G$DAC1H$0$0 == 0x00d3
                           0000D3   683 _DAC1H	=	0x00d3
                           0000D4   684 G$DAC0CN$0$0 == 0x00d4
                           0000D4   685 _DAC0CN	=	0x00d4
                           0000D4   686 G$DAC1CN$0$0 == 0x00d4
                           0000D4   687 _DAC1CN	=	0x00d4
                           0000D6   688 G$HVA0CN$0$0 == 0x00d6
                           0000D6   689 _HVA0CN	=	0x00d6
                           0000D8   690 G$PCA0CN$0$0 == 0x00d8
                           0000D8   691 _PCA0CN	=	0x00d8
                           0000D8   692 G$CAN0DATL$0$0 == 0x00d8
                           0000D8   693 _CAN0DATL	=	0x00d8
                           0000D8   694 G$P5$0$0 == 0x00d8
                           0000D8   695 _P5	=	0x00d8
                           0000D9   696 G$PCA0MD$0$0 == 0x00d9
                           0000D9   697 _PCA0MD	=	0x00d9
                           0000D9   698 G$CAN0DATH$0$0 == 0x00d9
                           0000D9   699 _CAN0DATH	=	0x00d9
                           0000DA   700 G$PCA0CPM0$0$0 == 0x00da
                           0000DA   701 _PCA0CPM0	=	0x00da
                           0000DA   702 G$CAN0ADR$0$0 == 0x00da
                           0000DA   703 _CAN0ADR	=	0x00da
                           0000DB   704 G$PCA0CPM1$0$0 == 0x00db
                           0000DB   705 _PCA0CPM1	=	0x00db
                           0000DB   706 G$CAN0TST$0$0 == 0x00db
                           0000DB   707 _CAN0TST	=	0x00db
                           0000DC   708 G$PCA0CPM2$0$0 == 0x00dc
                           0000DC   709 _PCA0CPM2	=	0x00dc
                           0000DD   710 G$PCA0CPM3$0$0 == 0x00dd
                           0000DD   711 _PCA0CPM3	=	0x00dd
                           0000DE   712 G$PCA0CPM4$0$0 == 0x00de
                           0000DE   713 _PCA0CPM4	=	0x00de
                           0000DF   714 G$PCA0CPM5$0$0 == 0x00df
                           0000DF   715 _PCA0CPM5	=	0x00df
                           0000E0   716 G$ACC$0$0 == 0x00e0
                           0000E0   717 _ACC	=	0x00e0
                           0000E1   718 G$PCA0CPL5$0$0 == 0x00e1
                           0000E1   719 _PCA0CPL5	=	0x00e1
                           0000E1   720 G$XBR0$0$0 == 0x00e1
                           0000E1   721 _XBR0	=	0x00e1
                           0000E2   722 G$PCA0CPH5$0$0 == 0x00e2
                           0000E2   723 _PCA0CPH5	=	0x00e2
                           0000E2   724 G$XBR1$0$0 == 0x00e2
                           0000E2   725 _XBR1	=	0x00e2
                           0000E3   726 G$XBR2$0$0 == 0x00e3
                           0000E3   727 _XBR2	=	0x00e3
                           0000E4   728 G$XBR3$0$0 == 0x00e4
                           0000E4   729 _XBR3	=	0x00e4
                           0000E6   730 G$EIE1$0$0 == 0x00e6
                           0000E6   731 _EIE1	=	0x00e6
                           0000E7   732 G$EIE2$0$0 == 0x00e7
                           0000E7   733 _EIE2	=	0x00e7
                           0000E8   734 G$ADC0CN$0$0 == 0x00e8
                           0000E8   735 _ADC0CN	=	0x00e8
                           0000E8   736 G$ADC2CN$0$0 == 0x00e8
                           0000E8   737 _ADC2CN	=	0x00e8
                           0000E8   738 G$P6$0$0 == 0x00e8
                           0000E8   739 _P6	=	0x00e8
                           0000E9   740 G$PCA0CPL2$0$0 == 0x00e9
                           0000E9   741 _PCA0CPL2	=	0x00e9
                           0000EA   742 G$PCA0CPH2$0$0 == 0x00ea
                           0000EA   743 _PCA0CPH2	=	0x00ea
                           0000EB   744 G$PCA0CPL3$0$0 == 0x00eb
                           0000EB   745 _PCA0CPL3	=	0x00eb
                           0000EC   746 G$PCA0CPH3$0$0 == 0x00ec
                           0000EC   747 _PCA0CPH3	=	0x00ec
                           0000ED   748 G$PCA0CPL4$0$0 == 0x00ed
                           0000ED   749 _PCA0CPL4	=	0x00ed
                           0000EE   750 G$PCA0CPH4$0$0 == 0x00ee
                           0000EE   751 _PCA0CPH4	=	0x00ee
                           0000EF   752 G$RSTSRC$0$0 == 0x00ef
                           0000EF   753 _RSTSRC	=	0x00ef
                           0000F0   754 G$B$0$0 == 0x00f0
                           0000F0   755 _B	=	0x00f0
                           0000F6   756 G$EIP1$0$0 == 0x00f6
                           0000F6   757 _EIP1	=	0x00f6
                           0000F7   758 G$EIP2$0$0 == 0x00f7
                           0000F7   759 _EIP2	=	0x00f7
                           0000F8   760 G$SPI0CN$0$0 == 0x00f8
                           0000F8   761 _SPI0CN	=	0x00f8
                           0000F8   762 G$CAN0CN$0$0 == 0x00f8
                           0000F8   763 _CAN0CN	=	0x00f8
                           0000F8   764 G$P7$0$0 == 0x00f8
                           0000F8   765 _P7	=	0x00f8
                           0000F9   766 G$PCA0L$0$0 == 0x00f9
                           0000F9   767 _PCA0L	=	0x00f9
                           0000FA   768 G$PCA0H$0$0 == 0x00fa
                           0000FA   769 _PCA0H	=	0x00fa
                           0000FB   770 G$PCA0CPL0$0$0 == 0x00fb
                           0000FB   771 _PCA0CPL0	=	0x00fb
                           0000FC   772 G$PCA0CPH0$0$0 == 0x00fc
                           0000FC   773 _PCA0CPH0	=	0x00fc
                           0000FD   774 G$PCA0CPL1$0$0 == 0x00fd
                           0000FD   775 _PCA0CPL1	=	0x00fd
                           0000FE   776 G$PCA0CPH1$0$0 == 0x00fe
                           0000FE   777 _PCA0CPH1	=	0x00fe
                           0000FF   778 G$WDTCN$0$0 == 0x00ff
                           0000FF   779 _WDTCN	=	0x00ff
                           00FAF9   780 G$PCA0$0$0 == 0xfaf9
                           00FAF9   781 _PCA0	=	0xfaf9
                           00FCFB   782 G$PCA0CP0$0$0 == 0xfcfb
                           00FCFB   783 _PCA0CP0	=	0xfcfb
                           00FEFD   784 G$PCA0CP1$0$0 == 0xfefd
                           00FEFD   785 _PCA0CP1	=	0xfefd
                           00EAE9   786 G$PCA0CP2$0$0 == 0xeae9
                           00EAE9   787 _PCA0CP2	=	0xeae9
                           00ECEB   788 G$PCA0CP3$0$0 == 0xeceb
                           00ECEB   789 _PCA0CP3	=	0xeceb
                           00EEED   790 G$PCA0CP4$0$0 == 0xeeed
                           00EEED   791 _PCA0CP4	=	0xeeed
                           00E2E1   792 G$PCA0CP5$0$0 == 0xe2e1
                           00E2E1   793 _PCA0CP5	=	0xe2e1
                           00D9D8   794 G$CAN0DAT$0$0 == 0xd9d8
                           00D9D8   795 _CAN0DAT	=	0xd9d8
                           00D3D2   796 G$DAC0$0$0 == 0xd3d2
                           00D3D2   797 _DAC0	=	0xd3d2
                           00D3D2   798 G$DAC1$0$0 == 0xd3d2
                           00D3D2   799 _DAC1	=	0xd3d2
                           00CBCA   800 G$RCAP2$0$0 == 0xcbca
                           00CBCA   801 _RCAP2	=	0xcbca
                           00CBCA   802 G$RCAP3$0$0 == 0xcbca
                           00CBCA   803 _RCAP3	=	0xcbca
                           00CBCA   804 G$RCAP4$0$0 == 0xcbca
                           00CBCA   805 _RCAP4	=	0xcbca
                           00CDCC   806 G$TMR2$0$0 == 0xcdcc
                           00CDCC   807 _TMR2	=	0xcdcc
                           00CDCC   808 G$TMR3$0$0 == 0xcdcc
                           00CDCC   809 _TMR3	=	0xcdcc
                           00CDCC   810 G$TMR4$0$0 == 0xcdcc
                           00CDCC   811 _TMR4	=	0xcdcc
                           00C5C4   812 G$ADC0GT$0$0 == 0xc5c4
                           00C5C4   813 _ADC0GT	=	0xc5c4
                           00C7C6   814 G$ADC0LT$0$0 == 0xc7c6
                           00C7C6   815 _ADC0LT	=	0xc7c6
                           00BFBE   816 G$ADC0$0$0 == 0xbfbe
                           00BFBE   817 _ADC0	=	0xbfbe
                           008382   818 G$DP$0$0 == 0x8382
                           008382   819 _DP	=	0x8382
                           0000A2   820 G$_XPAGE$0$0 == 0x00a2
                           0000A2   821 __XPAGE	=	0x00a2
                                    822 ;--------------------------------------------------------
                                    823 ; special function bits
                                    824 ;--------------------------------------------------------
                                    825 	.area RSEG    (ABS,DATA)
      000000                        826 	.org 0x0000
                           00008F   827 G$TF1$0$0 == 0x008f
                           00008F   828 _TF1	=	0x008f
                           00008E   829 G$TR1$0$0 == 0x008e
                           00008E   830 _TR1	=	0x008e
                           00008D   831 G$TF0$0$0 == 0x008d
                           00008D   832 _TF0	=	0x008d
                           00008C   833 G$TR0$0$0 == 0x008c
                           00008C   834 _TR0	=	0x008c
                           00008B   835 G$IE1$0$0 == 0x008b
                           00008B   836 _IE1	=	0x008b
                           00008A   837 G$IT1$0$0 == 0x008a
                           00008A   838 _IT1	=	0x008a
                           000089   839 G$IE0$0$0 == 0x0089
                           000089   840 _IE0	=	0x0089
                           000088   841 G$IT0$0$0 == 0x0088
                           000088   842 _IT0	=	0x0088
                           00008F   843 G$CP0EN$0$0 == 0x008f
                           00008F   844 _CP0EN	=	0x008f
                           00008E   845 G$CP0OUT$0$0 == 0x008e
                           00008E   846 _CP0OUT	=	0x008e
                           00008D   847 G$CP0RIF$0$0 == 0x008d
                           00008D   848 _CP0RIF	=	0x008d
                           00008C   849 G$CP0FIF$0$0 == 0x008c
                           00008C   850 _CP0FIF	=	0x008c
                           00008B   851 G$CP0HYP1$0$0 == 0x008b
                           00008B   852 _CP0HYP1	=	0x008b
                           00008A   853 G$CP0HYP0$0$0 == 0x008a
                           00008A   854 _CP0HYP0	=	0x008a
                           000089   855 G$CP0HYN1$0$0 == 0x0089
                           000089   856 _CP0HYN1	=	0x0089
                           000088   857 G$CP0HYN0$0$0 == 0x0088
                           000088   858 _CP0HYN0	=	0x0088
                           00008F   859 G$CP1EN$0$0 == 0x008f
                           00008F   860 _CP1EN	=	0x008f
                           00008E   861 G$CP1OUT$0$0 == 0x008e
                           00008E   862 _CP1OUT	=	0x008e
                           00008D   863 G$CP1RIF$0$0 == 0x008d
                           00008D   864 _CP1RIF	=	0x008d
                           00008C   865 G$CP1FIF$0$0 == 0x008c
                           00008C   866 _CP1FIF	=	0x008c
                           00008B   867 G$CP1HYP1$0$0 == 0x008b
                           00008B   868 _CP1HYP1	=	0x008b
                           00008A   869 G$CP1HYP0$0$0 == 0x008a
                           00008A   870 _CP1HYP0	=	0x008a
                           000089   871 G$CP1HYN1$0$0 == 0x0089
                           000089   872 _CP1HYN1	=	0x0089
                           000088   873 G$CP1HYN0$0$0 == 0x0088
                           000088   874 _CP1HYN0	=	0x0088
                           00008F   875 G$CP2EN$0$0 == 0x008f
                           00008F   876 _CP2EN	=	0x008f
                           00008E   877 G$CP2OUT$0$0 == 0x008e
                           00008E   878 _CP2OUT	=	0x008e
                           00008D   879 G$CP2RIF$0$0 == 0x008d
                           00008D   880 _CP2RIF	=	0x008d
                           00008C   881 G$CP2FIF$0$0 == 0x008c
                           00008C   882 _CP2FIF	=	0x008c
                           00008B   883 G$CP2HYP1$0$0 == 0x008b
                           00008B   884 _CP2HYP1	=	0x008b
                           00008A   885 G$CP2HYP0$0$0 == 0x008a
                           00008A   886 _CP2HYP0	=	0x008a
                           000089   887 G$CP2HYN1$0$0 == 0x0089
                           000089   888 _CP2HYN1	=	0x0089
                           000088   889 G$CP2HYN0$0$0 == 0x0088
                           000088   890 _CP2HYN0	=	0x0088
                           00009F   891 G$SM00$0$0 == 0x009f
                           00009F   892 _SM00	=	0x009f
                           00009E   893 G$SM10$0$0 == 0x009e
                           00009E   894 _SM10	=	0x009e
                           00009D   895 G$SM20$0$0 == 0x009d
                           00009D   896 _SM20	=	0x009d
                           00009C   897 G$REN0$0$0 == 0x009c
                           00009C   898 _REN0	=	0x009c
                           00009B   899 G$TB80$0$0 == 0x009b
                           00009B   900 _TB80	=	0x009b
                           00009A   901 G$RB80$0$0 == 0x009a
                           00009A   902 _RB80	=	0x009a
                           000099   903 G$TI0$0$0 == 0x0099
                           000099   904 _TI0	=	0x0099
                           000098   905 G$RI0$0$0 == 0x0098
                           000098   906 _RI0	=	0x0098
                           00009F   907 G$S1MODE$0$0 == 0x009f
                           00009F   908 _S1MODE	=	0x009f
                           00009D   909 G$MCE1$0$0 == 0x009d
                           00009D   910 _MCE1	=	0x009d
                           00009C   911 G$REN1$0$0 == 0x009c
                           00009C   912 _REN1	=	0x009c
                           00009B   913 G$TB81$0$0 == 0x009b
                           00009B   914 _TB81	=	0x009b
                           00009A   915 G$RB81$0$0 == 0x009a
                           00009A   916 _RB81	=	0x009a
                           000099   917 G$TI1$0$0 == 0x0099
                           000099   918 _TI1	=	0x0099
                           000098   919 G$RI1$0$0 == 0x0098
                           000098   920 _RI1	=	0x0098
                           0000AF   921 G$EA$0$0 == 0x00af
                           0000AF   922 _EA	=	0x00af
                           0000AD   923 G$ET2$0$0 == 0x00ad
                           0000AD   924 _ET2	=	0x00ad
                           0000AC   925 G$ES0$0$0 == 0x00ac
                           0000AC   926 _ES0	=	0x00ac
                           0000AB   927 G$ET1$0$0 == 0x00ab
                           0000AB   928 _ET1	=	0x00ab
                           0000AA   929 G$EX1$0$0 == 0x00aa
                           0000AA   930 _EX1	=	0x00aa
                           0000A9   931 G$ET0$0$0 == 0x00a9
                           0000A9   932 _ET0	=	0x00a9
                           0000A8   933 G$EX0$0$0 == 0x00a8
                           0000A8   934 _EX0	=	0x00a8
                           0000BD   935 G$PT2$0$0 == 0x00bd
                           0000BD   936 _PT2	=	0x00bd
                           0000BC   937 G$PS0$0$0 == 0x00bc
                           0000BC   938 _PS0	=	0x00bc
                           0000BB   939 G$PT1$0$0 == 0x00bb
                           0000BB   940 _PT1	=	0x00bb
                           0000BA   941 G$PX1$0$0 == 0x00ba
                           0000BA   942 _PX1	=	0x00ba
                           0000B9   943 G$PT0$0$0 == 0x00b9
                           0000B9   944 _PT0	=	0x00b9
                           0000B8   945 G$PX0$0$0 == 0x00b8
                           0000B8   946 _PX0	=	0x00b8
                           0000C7   947 G$BUSY$0$0 == 0x00c7
                           0000C7   948 _BUSY	=	0x00c7
                           0000C6   949 G$ENSMB$0$0 == 0x00c6
                           0000C6   950 _ENSMB	=	0x00c6
                           0000C5   951 G$STA$0$0 == 0x00c5
                           0000C5   952 _STA	=	0x00c5
                           0000C4   953 G$STO$0$0 == 0x00c4
                           0000C4   954 _STO	=	0x00c4
                           0000C3   955 G$SI$0$0 == 0x00c3
                           0000C3   956 _SI	=	0x00c3
                           0000C2   957 G$AA$0$0 == 0x00c2
                           0000C2   958 _AA	=	0x00c2
                           0000C1   959 G$SMBFTE$0$0 == 0x00c1
                           0000C1   960 _SMBFTE	=	0x00c1
                           0000C0   961 G$SMBTOE$0$0 == 0x00c0
                           0000C0   962 _SMBTOE	=	0x00c0
                           0000C7   963 G$BOFF$0$0 == 0x00c7
                           0000C7   964 _BOFF	=	0x00c7
                           0000C6   965 G$EWARN$0$0 == 0x00c6
                           0000C6   966 _EWARN	=	0x00c6
                           0000C5   967 G$EPASS$0$0 == 0x00c5
                           0000C5   968 _EPASS	=	0x00c5
                           0000C4   969 G$RXOK$0$0 == 0x00c4
                           0000C4   970 _RXOK	=	0x00c4
                           0000C3   971 G$TXOK$0$0 == 0x00c3
                           0000C3   972 _TXOK	=	0x00c3
                           0000C2   973 G$LEC2$0$0 == 0x00c2
                           0000C2   974 _LEC2	=	0x00c2
                           0000C1   975 G$LEC1$0$0 == 0x00c1
                           0000C1   976 _LEC1	=	0x00c1
                           0000C0   977 G$LEC0$0$0 == 0x00c0
                           0000C0   978 _LEC0	=	0x00c0
                           0000CF   979 G$TF2$0$0 == 0x00cf
                           0000CF   980 _TF2	=	0x00cf
                           0000CE   981 G$EXF2$0$0 == 0x00ce
                           0000CE   982 _EXF2	=	0x00ce
                           0000CB   983 G$EXEN2$0$0 == 0x00cb
                           0000CB   984 _EXEN2	=	0x00cb
                           0000CA   985 G$TR2$0$0 == 0x00ca
                           0000CA   986 _TR2	=	0x00ca
                           0000C9   987 G$CT2$0$0 == 0x00c9
                           0000C9   988 _CT2	=	0x00c9
                           0000C8   989 G$CPRL2$0$0 == 0x00c8
                           0000C8   990 _CPRL2	=	0x00c8
                           0000CF   991 G$TF3$0$0 == 0x00cf
                           0000CF   992 _TF3	=	0x00cf
                           0000CE   993 G$EXF3$0$0 == 0x00ce
                           0000CE   994 _EXF3	=	0x00ce
                           0000CB   995 G$EXEN3$0$0 == 0x00cb
                           0000CB   996 _EXEN3	=	0x00cb
                           0000CA   997 G$TR3$0$0 == 0x00ca
                           0000CA   998 _TR3	=	0x00ca
                           0000C9   999 G$CT3$0$0 == 0x00c9
                           0000C9  1000 _CT3	=	0x00c9
                           0000C8  1001 G$CPRL3$0$0 == 0x00c8
                           0000C8  1002 _CPRL3	=	0x00c8
                           0000CF  1003 G$TF4$0$0 == 0x00cf
                           0000CF  1004 _TF4	=	0x00cf
                           0000CE  1005 G$EXF4$0$0 == 0x00ce
                           0000CE  1006 _EXF4	=	0x00ce
                           0000CB  1007 G$EXEN4$0$0 == 0x00cb
                           0000CB  1008 _EXEN4	=	0x00cb
                           0000CA  1009 G$TR4$0$0 == 0x00ca
                           0000CA  1010 _TR4	=	0x00ca
                           0000C9  1011 G$CT4$0$0 == 0x00c9
                           0000C9  1012 _CT4	=	0x00c9
                           0000C8  1013 G$CPRL4$0$0 == 0x00c8
                           0000C8  1014 _CPRL4	=	0x00c8
                           0000D7  1015 G$CY$0$0 == 0x00d7
                           0000D7  1016 _CY	=	0x00d7
                           0000D6  1017 G$AC$0$0 == 0x00d6
                           0000D6  1018 _AC	=	0x00d6
                           0000D5  1019 G$F0$0$0 == 0x00d5
                           0000D5  1020 _F0	=	0x00d5
                           0000D4  1021 G$RS1$0$0 == 0x00d4
                           0000D4  1022 _RS1	=	0x00d4
                           0000D3  1023 G$RS0$0$0 == 0x00d3
                           0000D3  1024 _RS0	=	0x00d3
                           0000D2  1025 G$OV$0$0 == 0x00d2
                           0000D2  1026 _OV	=	0x00d2
                           0000D1  1027 G$F1$0$0 == 0x00d1
                           0000D1  1028 _F1	=	0x00d1
                           0000D0  1029 G$P$0$0 == 0x00d0
                           0000D0  1030 _P	=	0x00d0
                           0000DF  1031 G$CF$0$0 == 0x00df
                           0000DF  1032 _CF	=	0x00df
                           0000DE  1033 G$CR$0$0 == 0x00de
                           0000DE  1034 _CR	=	0x00de
                           0000DD  1035 G$CCF5$0$0 == 0x00dd
                           0000DD  1036 _CCF5	=	0x00dd
                           0000DC  1037 G$CCF4$0$0 == 0x00dc
                           0000DC  1038 _CCF4	=	0x00dc
                           0000DB  1039 G$CCF3$0$0 == 0x00db
                           0000DB  1040 _CCF3	=	0x00db
                           0000DA  1041 G$CCF2$0$0 == 0x00da
                           0000DA  1042 _CCF2	=	0x00da
                           0000D9  1043 G$CCF1$0$0 == 0x00d9
                           0000D9  1044 _CCF1	=	0x00d9
                           0000D8  1045 G$CCF0$0$0 == 0x00d8
                           0000D8  1046 _CCF0	=	0x00d8
                           0000EF  1047 G$AD0EN$0$0 == 0x00ef
                           0000EF  1048 _AD0EN	=	0x00ef
                           0000EE  1049 G$AD0TM$0$0 == 0x00ee
                           0000EE  1050 _AD0TM	=	0x00ee
                           0000ED  1051 G$AD0INT$0$0 == 0x00ed
                           0000ED  1052 _AD0INT	=	0x00ed
                           0000EC  1053 G$AD0BUSY$0$0 == 0x00ec
                           0000EC  1054 _AD0BUSY	=	0x00ec
                           0000EB  1055 G$AD0CM1$0$0 == 0x00eb
                           0000EB  1056 _AD0CM1	=	0x00eb
                           0000EA  1057 G$AD0CM0$0$0 == 0x00ea
                           0000EA  1058 _AD0CM0	=	0x00ea
                           0000E9  1059 G$AD0WINT$0$0 == 0x00e9
                           0000E9  1060 _AD0WINT	=	0x00e9
                           0000E8  1061 G$AD0LJST$0$0 == 0x00e8
                           0000E8  1062 _AD0LJST	=	0x00e8
                           0000EF  1063 G$AD2EN$0$0 == 0x00ef
                           0000EF  1064 _AD2EN	=	0x00ef
                           0000EE  1065 G$AD2TM$0$0 == 0x00ee
                           0000EE  1066 _AD2TM	=	0x00ee
                           0000ED  1067 G$AD2INT$0$0 == 0x00ed
                           0000ED  1068 _AD2INT	=	0x00ed
                           0000EC  1069 G$AD2BUSY$0$0 == 0x00ec
                           0000EC  1070 _AD2BUSY	=	0x00ec
                           0000EB  1071 G$AD2CM2$0$0 == 0x00eb
                           0000EB  1072 _AD2CM2	=	0x00eb
                           0000EA  1073 G$AD2CM1$0$0 == 0x00ea
                           0000EA  1074 _AD2CM1	=	0x00ea
                           0000E9  1075 G$AD2CM0$0$0 == 0x00e9
                           0000E9  1076 _AD2CM0	=	0x00e9
                           0000E8  1077 G$AD2WINT$0$0 == 0x00e8
                           0000E8  1078 _AD2WINT	=	0x00e8
                           0000FF  1079 G$SPIF$0$0 == 0x00ff
                           0000FF  1080 _SPIF	=	0x00ff
                           0000FE  1081 G$WCOL$0$0 == 0x00fe
                           0000FE  1082 _WCOL	=	0x00fe
                           0000FD  1083 G$MODF$0$0 == 0x00fd
                           0000FD  1084 _MODF	=	0x00fd
                           0000FC  1085 G$RXOVRN$0$0 == 0x00fc
                           0000FC  1086 _RXOVRN	=	0x00fc
                           0000FB  1087 G$NSSMD1$0$0 == 0x00fb
                           0000FB  1088 _NSSMD1	=	0x00fb
                           0000FA  1089 G$NSSMD0$0$0 == 0x00fa
                           0000FA  1090 _NSSMD0	=	0x00fa
                           0000F9  1091 G$TXBMT$0$0 == 0x00f9
                           0000F9  1092 _TXBMT	=	0x00f9
                           0000F8  1093 G$SPIEN$0$0 == 0x00f8
                           0000F8  1094 _SPIEN	=	0x00f8
                           0000F8  1095 G$CANINIT$0$0 == 0x00f8
                           0000F8  1096 _CANINIT	=	0x00f8
                           0000F9  1097 G$CANIE$0$0 == 0x00f9
                           0000F9  1098 _CANIE	=	0x00f9
                           0000FA  1099 G$CANSIE$0$0 == 0x00fa
                           0000FA  1100 _CANSIE	=	0x00fa
                           0000FB  1101 G$CANEIE$0$0 == 0x00fb
                           0000FB  1102 _CANEIE	=	0x00fb
                           0000FC  1103 G$CANIF$0$0 == 0x00fc
                           0000FC  1104 _CANIF	=	0x00fc
                           0000FD  1105 G$CANDAR$0$0 == 0x00fd
                           0000FD  1106 _CANDAR	=	0x00fd
                           0000FE  1107 G$CANCCE$0$0 == 0x00fe
                           0000FE  1108 _CANCCE	=	0x00fe
                           0000FF  1109 G$CANTEST$0$0 == 0x00ff
                           0000FF  1110 _CANTEST	=	0x00ff
                           000080  1111 G$P0_0$0$0 == 0x0080
                           000080  1112 _P0_0	=	0x0080
                           000081  1113 G$P0_1$0$0 == 0x0081
                           000081  1114 _P0_1	=	0x0081
                           000082  1115 G$P0_2$0$0 == 0x0082
                           000082  1116 _P0_2	=	0x0082
                           000083  1117 G$P0_3$0$0 == 0x0083
                           000083  1118 _P0_3	=	0x0083
                           000084  1119 G$P0_4$0$0 == 0x0084
                           000084  1120 _P0_4	=	0x0084
                           000085  1121 G$P0_5$0$0 == 0x0085
                           000085  1122 _P0_5	=	0x0085
                           000086  1123 G$P0_6$0$0 == 0x0086
                           000086  1124 _P0_6	=	0x0086
                           000087  1125 G$P0_7$0$0 == 0x0087
                           000087  1126 _P0_7	=	0x0087
                           000090  1127 G$P1_0$0$0 == 0x0090
                           000090  1128 _P1_0	=	0x0090
                           000091  1129 G$P1_1$0$0 == 0x0091
                           000091  1130 _P1_1	=	0x0091
                           000092  1131 G$P1_2$0$0 == 0x0092
                           000092  1132 _P1_2	=	0x0092
                           000093  1133 G$P1_3$0$0 == 0x0093
                           000093  1134 _P1_3	=	0x0093
                           000094  1135 G$P1_4$0$0 == 0x0094
                           000094  1136 _P1_4	=	0x0094
                           000095  1137 G$P1_5$0$0 == 0x0095
                           000095  1138 _P1_5	=	0x0095
                           000096  1139 G$P1_6$0$0 == 0x0096
                           000096  1140 _P1_6	=	0x0096
                           000097  1141 G$P1_7$0$0 == 0x0097
                           000097  1142 _P1_7	=	0x0097
                           0000A0  1143 G$P2_0$0$0 == 0x00a0
                           0000A0  1144 _P2_0	=	0x00a0
                           0000A1  1145 G$P2_1$0$0 == 0x00a1
                           0000A1  1146 _P2_1	=	0x00a1
                           0000A2  1147 G$P2_2$0$0 == 0x00a2
                           0000A2  1148 _P2_2	=	0x00a2
                           0000A3  1149 G$P2_3$0$0 == 0x00a3
                           0000A3  1150 _P2_3	=	0x00a3
                           0000A4  1151 G$P2_4$0$0 == 0x00a4
                           0000A4  1152 _P2_4	=	0x00a4
                           0000A5  1153 G$P2_5$0$0 == 0x00a5
                           0000A5  1154 _P2_5	=	0x00a5
                           0000A6  1155 G$P2_6$0$0 == 0x00a6
                           0000A6  1156 _P2_6	=	0x00a6
                           0000A7  1157 G$P2_7$0$0 == 0x00a7
                           0000A7  1158 _P2_7	=	0x00a7
                           0000B0  1159 G$P3_0$0$0 == 0x00b0
                           0000B0  1160 _P3_0	=	0x00b0
                           0000B1  1161 G$P3_1$0$0 == 0x00b1
                           0000B1  1162 _P3_1	=	0x00b1
                           0000B2  1163 G$P3_2$0$0 == 0x00b2
                           0000B2  1164 _P3_2	=	0x00b2
                           0000B3  1165 G$P3_3$0$0 == 0x00b3
                           0000B3  1166 _P3_3	=	0x00b3
                           0000B4  1167 G$P3_4$0$0 == 0x00b4
                           0000B4  1168 _P3_4	=	0x00b4
                           0000B5  1169 G$P3_5$0$0 == 0x00b5
                           0000B5  1170 _P3_5	=	0x00b5
                           0000B6  1171 G$P3_6$0$0 == 0x00b6
                           0000B6  1172 _P3_6	=	0x00b6
                           0000B7  1173 G$P3_7$0$0 == 0x00b7
                           0000B7  1174 _P3_7	=	0x00b7
                           0000C8  1175 G$P4_0$0$0 == 0x00c8
                           0000C8  1176 _P4_0	=	0x00c8
                           0000C9  1177 G$P4_1$0$0 == 0x00c9
                           0000C9  1178 _P4_1	=	0x00c9
                           0000CA  1179 G$P4_2$0$0 == 0x00ca
                           0000CA  1180 _P4_2	=	0x00ca
                           0000CB  1181 G$P4_3$0$0 == 0x00cb
                           0000CB  1182 _P4_3	=	0x00cb
                           0000CC  1183 G$P4_4$0$0 == 0x00cc
                           0000CC  1184 _P4_4	=	0x00cc
                           0000CD  1185 G$P4_5$0$0 == 0x00cd
                           0000CD  1186 _P4_5	=	0x00cd
                           0000CE  1187 G$P4_6$0$0 == 0x00ce
                           0000CE  1188 _P4_6	=	0x00ce
                           0000CF  1189 G$P4_7$0$0 == 0x00cf
                           0000CF  1190 _P4_7	=	0x00cf
                           0000D8  1191 G$P5_0$0$0 == 0x00d8
                           0000D8  1192 _P5_0	=	0x00d8
                           0000D9  1193 G$P5_1$0$0 == 0x00d9
                           0000D9  1194 _P5_1	=	0x00d9
                           0000DA  1195 G$P5_2$0$0 == 0x00da
                           0000DA  1196 _P5_2	=	0x00da
                           0000DB  1197 G$P5_3$0$0 == 0x00db
                           0000DB  1198 _P5_3	=	0x00db
                           0000DC  1199 G$P5_4$0$0 == 0x00dc
                           0000DC  1200 _P5_4	=	0x00dc
                           0000DD  1201 G$P5_5$0$0 == 0x00dd
                           0000DD  1202 _P5_5	=	0x00dd
                           0000DE  1203 G$P5_6$0$0 == 0x00de
                           0000DE  1204 _P5_6	=	0x00de
                           0000DF  1205 G$P5_7$0$0 == 0x00df
                           0000DF  1206 _P5_7	=	0x00df
                           0000E8  1207 G$P6_0$0$0 == 0x00e8
                           0000E8  1208 _P6_0	=	0x00e8
                           0000E9  1209 G$P6_1$0$0 == 0x00e9
                           0000E9  1210 _P6_1	=	0x00e9
                           0000EA  1211 G$P6_2$0$0 == 0x00ea
                           0000EA  1212 _P6_2	=	0x00ea
                           0000EB  1213 G$P6_3$0$0 == 0x00eb
                           0000EB  1214 _P6_3	=	0x00eb
                           0000EC  1215 G$P6_4$0$0 == 0x00ec
                           0000EC  1216 _P6_4	=	0x00ec
                           0000ED  1217 G$P6_5$0$0 == 0x00ed
                           0000ED  1218 _P6_5	=	0x00ed
                           0000EE  1219 G$P6_6$0$0 == 0x00ee
                           0000EE  1220 _P6_6	=	0x00ee
                           0000EF  1221 G$P6_7$0$0 == 0x00ef
                           0000EF  1222 _P6_7	=	0x00ef
                           0000F8  1223 G$P7_0$0$0 == 0x00f8
                           0000F8  1224 _P7_0	=	0x00f8
                           0000F9  1225 G$P7_1$0$0 == 0x00f9
                           0000F9  1226 _P7_1	=	0x00f9
                           0000FA  1227 G$P7_2$0$0 == 0x00fa
                           0000FA  1228 _P7_2	=	0x00fa
                           0000FB  1229 G$P7_3$0$0 == 0x00fb
                           0000FB  1230 _P7_3	=	0x00fb
                           0000FC  1231 G$P7_4$0$0 == 0x00fc
                           0000FC  1232 _P7_4	=	0x00fc
                           0000FD  1233 G$P7_5$0$0 == 0x00fd
                           0000FD  1234 _P7_5	=	0x00fd
                           0000FE  1235 G$P7_6$0$0 == 0x00fe
                           0000FE  1236 _P7_6	=	0x00fe
                           0000FF  1237 G$P7_7$0$0 == 0x00ff
                           0000FF  1238 _P7_7	=	0x00ff
                                   1239 ;--------------------------------------------------------
                                   1240 ; overlayable register banks
                                   1241 ;--------------------------------------------------------
                                   1242 	.area REG_BANK_0	(REL,OVR,DATA)
      000000                       1243 	.ds 8
                                   1244 ;--------------------------------------------------------
                                   1245 ; overlayable bit register bank
                                   1246 ;--------------------------------------------------------
                                   1247 	.area BIT_BANK	(REL,OVR,DATA)
      000023                       1248 bits:
      000023                       1249 	.ds 1
                           008000  1250 	b0 = bits[0]
                           008100  1251 	b1 = bits[1]
                           008200  1252 	b2 = bits[2]
                           008300  1253 	b3 = bits[3]
                           008400  1254 	b4 = bits[4]
                           008500  1255 	b5 = bits[5]
                           008600  1256 	b6 = bits[6]
                           008700  1257 	b7 = bits[7]
                                   1258 ;--------------------------------------------------------
                                   1259 ; internal ram data
                                   1260 ;--------------------------------------------------------
                                   1261 	.area DSEG    (DATA)
                           000000  1262 G$conta_caractere$0$0==.
      000024                       1263 _conta_caractere::
      000024                       1264 	.ds 1
                           000001  1265 G$saida$0$0==.
      000025                       1266 _saida::
      000025                       1267 	.ds 6
                           000007  1268 Lmain.le_voltagem$ganho$1$76==.
      00002B                       1269 _le_voltagem_PARM_2:
      00002B                       1270 	.ds 1
                           000008  1271 G$end_fim_ram$0$0==.
      00002C                       1272 _end_fim_ram::
      00002C                       1273 	.ds 2
                           00000A  1274 G$relogio$0$0==.
      00002E                       1275 _relogio::
      00002E                       1276 	.ds 7
                           000011  1277 Lmain.print_relogio_terminal$sloc0$1$0==.
      000035                       1278 _print_relogio_terminal_sloc0_1_0:
      000035                       1279 	.ds 2
                           000013  1280 Lmain.print_relogio_terminal$sloc1$1$0==.
      000037                       1281 _print_relogio_terminal_sloc1_1_0:
      000037                       1282 	.ds 2
                           000015  1283 Lmain.print_relogio_terminal$sloc2$1$0==.
      000039                       1284 _print_relogio_terminal_sloc2_1_0:
      000039                       1285 	.ds 2
                           000017  1286 Lmain.print_relogio_glcd$sloc0$1$0==.
      00003B                       1287 _print_relogio_glcd_sloc0_1_0:
      00003B                       1288 	.ds 2
                           000019  1289 Lmain.print_relogio_glcd$sloc1$1$0==.
      00003D                       1290 _print_relogio_glcd_sloc1_1_0:
      00003D                       1291 	.ds 2
                           00001B  1292 Lmain.print_relogio_glcd$sloc2$1$0==.
      00003F                       1293 _print_relogio_glcd_sloc2_1_0:
      00003F                       1294 	.ds 2
                           00001D  1295 Lmain.demonstra_amostras$i$1$102==.
      000041                       1296 _demonstra_amostras_i_1_102:
      000041                       1297 	.ds 2
                           00001F  1298 Lmain.demonstra_amostras$sloc0$1$0==.
      000043                       1299 _demonstra_amostras_sloc0_1_0:
      000043                       1300 	.ds 2
                           000021  1301 Lmain.demonstra_amostras$sloc1$1$0==.
      000045                       1302 _demonstra_amostras_sloc1_1_0:
      000045                       1303 	.ds 2
                           000023  1304 G$tecla$0$0==.
      000047                       1305 _tecla::
      000047                       1306 	.ds 1
                           000024  1307 Lmain.ligar_buzzer$meio_periodo$1$109==.
      000048                       1308 _ligar_buzzer_PARM_2:
      000048                       1309 	.ds 2
                           000026  1310 Lmain.imprime_terminal_tempo_real$sloc0$1$0==.
      00004A                       1311 _imprime_terminal_tempo_real_sloc0_1_0:
      00004A                       1312 	.ds 2
                           000028  1313 Lmain.imprime_terminal_tempo_real$sloc1$1$0==.
      00004C                       1314 _imprime_terminal_tempo_real_sloc1_1_0:
      00004C                       1315 	.ds 2
                                   1316 ;--------------------------------------------------------
                                   1317 ; overlayable items in internal ram 
                                   1318 ;--------------------------------------------------------
                                   1319 	.area	OSEG    (OVR,DATA)
                                   1320 	.area	OSEG    (OVR,DATA)
                                   1321 	.area	OSEG    (OVR,DATA)
                                   1322 	.area	OSEG    (OVR,DATA)
                                   1323 	.area	OSEG    (OVR,DATA)
                                   1324 	.area	OSEG    (OVR,DATA)
                           000000  1325 Lmain.le_adc0$ganho$1$74==.
      00000F                       1326 _le_adc0_PARM_2:
      00000F                       1327 	.ds 1
                           000001  1328 Lmain.le_adc0$indice_high$1$74==.
      000010                       1329 _le_adc0_PARM_3:
      000010                       1330 	.ds 1
                           000002  1331 Lmain.le_adc0$indice_low$1$74==.
      000011                       1332 _le_adc0_PARM_4:
      000011                       1333 	.ds 1
                                   1334 	.area	OSEG    (OVR,DATA)
                           000000  1335 Lmain.esc_RAM_SPI$dado$1$80==.
      00000F                       1336 _esc_RAM_SPI_PARM_2:
      00000F                       1337 	.ds 1
                                   1338 	.area	OSEG    (OVR,DATA)
                                   1339 	.area	OSEG    (OVR,DATA)
                           000000  1340 Lmain.ini_relogio$mes$1$94==.
      00000F                       1341 _ini_relogio_PARM_2:
      00000F                       1342 	.ds 1
                           000001  1343 Lmain.ini_relogio$ano$1$94==.
      000010                       1344 _ini_relogio_PARM_3:
      000010                       1345 	.ds 1
                           000002  1346 Lmain.ini_relogio$hora$1$94==.
      000011                       1347 _ini_relogio_PARM_4:
      000011                       1348 	.ds 1
                           000003  1349 Lmain.ini_relogio$minuto$1$94==.
      000012                       1350 _ini_relogio_PARM_5:
      000012                       1351 	.ds 1
                           000004  1352 Lmain.ini_relogio$segundo$1$94==.
      000013                       1353 _ini_relogio_PARM_6:
      000013                       1354 	.ds 1
                                   1355 ;--------------------------------------------------------
                                   1356 ; Stack segment in internal ram 
                                   1357 ;--------------------------------------------------------
                                   1358 	.area	SSEG
      00004E                       1359 __start__stack:
      00004E                       1360 	.ds	1
                                   1361 
                                   1362 ;--------------------------------------------------------
                                   1363 ; indirectly addressable internal ram data
                                   1364 ;--------------------------------------------------------
                                   1365 	.area ISEG    (DATA)
                                   1366 ;--------------------------------------------------------
                                   1367 ; absolute internal ram data
                                   1368 ;--------------------------------------------------------
                                   1369 	.area IABS    (ABS,DATA)
                                   1370 	.area IABS    (ABS,DATA)
                                   1371 ;--------------------------------------------------------
                                   1372 ; bit data
                                   1373 ;--------------------------------------------------------
                                   1374 	.area BSEG    (BIT)
                           000000  1375 G$terminal_ativo$0$0==.
      000000                       1376 _terminal_ativo::
      000000                       1377 	.ds 1
                           000001  1378 Lmain.le_glcd$cd$1$27==.
      000001                       1379 _le_glcd_PARM_1:
      000001                       1380 	.ds 1
                           000002  1381 Lmain.le_glcd$cs$1$27==.
      000002                       1382 _le_glcd_PARM_2:
      000002                       1383 	.ds 1
                           000003  1384 Lmain.esc_glcd$cd$1$29==.
      000003                       1385 _esc_glcd_PARM_2:
      000003                       1386 	.ds 1
                           000004  1387 Lmain.esc_glcd$cs$1$29==.
      000004                       1388 _esc_glcd_PARM_3:
      000004                       1389 	.ds 1
                           000005  1390 Lmain.ini_glcd$sloc0$1$0==.
      000005                       1391 _ini_glcd_sloc0_1_0:
      000005                       1392 	.ds 1
                           000006  1393 Lmain.conf_Y$cs$1$33==.
      000006                       1394 _conf_Y_PARM_2:
      000006                       1395 	.ds 1
                           000007  1396 Lmain.conf_pag$cs$1$35==.
      000007                       1397 _conf_pag_PARM_2:
      000007                       1398 	.ds 1
                           000008  1399 Lmain.limpa_glcd$cs$1$37==.
      000008                       1400 _limpa_glcd_PARM_1:
      000008                       1401 	.ds 1
                           000009  1402 Lmain.escreve_caractere$cs$1$45==.
      000009                       1403 _escreve_caractere_PARM_2:
      000009                       1404 	.ds 1
                           00000A  1405 Lmain.putchar$lado$1$48==.
      00000A                       1406 _putchar_lado_1_48:
      00000A                       1407 	.ds 1
                           00000B  1408 G$transmissao_dht11$0$0==.
      00000B                       1409 _transmissao_dht11::
      00000B                       1410 	.ds 1
                           00000C  1411 G$flag_tecla$0$0==.
      00000C                       1412 _flag_tecla::
      00000C                       1413 	.ds 1
                                   1414 ;--------------------------------------------------------
                                   1415 ; paged external ram data
                                   1416 ;--------------------------------------------------------
                                   1417 	.area PSEG    (PAG,XDATA)
                                   1418 ;--------------------------------------------------------
                                   1419 ; external ram data
                                   1420 ;--------------------------------------------------------
                                   1421 	.area XSEG    (XDATA)
                                   1422 ;--------------------------------------------------------
                                   1423 ; absolute external ram data
                                   1424 ;--------------------------------------------------------
                                   1425 	.area XABS    (ABS,XDATA)
                                   1426 ;--------------------------------------------------------
                                   1427 ; external initialized ram data
                                   1428 ;--------------------------------------------------------
                                   1429 	.area XISEG   (XDATA)
                                   1430 	.area HOME    (CODE)
                                   1431 	.area GSINIT0 (CODE)
                                   1432 	.area GSINIT1 (CODE)
                                   1433 	.area GSINIT2 (CODE)
                                   1434 	.area GSINIT3 (CODE)
                                   1435 	.area GSINIT4 (CODE)
                                   1436 	.area GSINIT5 (CODE)
                                   1437 	.area GSINIT  (CODE)
                                   1438 	.area GSFINAL (CODE)
                                   1439 	.area CSEG    (CODE)
                                   1440 ;--------------------------------------------------------
                                   1441 ; interrupt vector 
                                   1442 ;--------------------------------------------------------
                                   1443 	.area HOME    (CODE)
      000000                       1444 __interrupt_vect:
      000000 02 00 31         [24] 1445 	ljmp	__sdcc_gsinit_startup
      000003 32               [24] 1446 	reti
      000004                       1447 	.ds	7
      00000B 32               [24] 1448 	reti
      00000C                       1449 	.ds	7
      000013 32               [24] 1450 	reti
      000014                       1451 	.ds	7
      00001B 32               [24] 1452 	reti
      00001C                       1453 	.ds	7
      000023 02 0A B9         [24] 1454 	ljmp	_isr_UART0
      000026                       1455 	.ds	5
      00002B 02 09 B5         [24] 1456 	ljmp	_isr_tempo
                                   1457 ;--------------------------------------------------------
                                   1458 ; global & static initialisations
                                   1459 ;--------------------------------------------------------
                                   1460 	.area HOME    (CODE)
                                   1461 	.area GSINIT  (CODE)
                                   1462 	.area GSFINAL (CODE)
                                   1463 	.area GSINIT  (CODE)
                                   1464 	.globl __sdcc_gsinit_startup
                                   1465 	.globl __sdcc_program_startup
                                   1466 	.globl __start__stack
                                   1467 	.globl __mcs51_genXINIT
                                   1468 	.globl __mcs51_genXRAMCLEAR
                                   1469 	.globl __mcs51_genRAMCLEAR
                           000000  1470 	C$glcd.c$21$1$123 ==.
                                   1471 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:21: volatile unsigned char conta_caractere = 0;
      00008A 75 24 00         [24] 1472 	mov	_conta_caractere,#0x00
                           000003  1473 	C$ram_spi.c$15$1$123 ==.
                                   1474 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:15: volatile unsigned int end_fim_ram = 0;
      00008D E4               [12] 1475 	clr	a
      00008E F5 2C            [12] 1476 	mov	_end_fim_ram,a
      000090 F5 2D            [12] 1477 	mov	(_end_fim_ram + 1),a
                           000008  1478 	C$tempo.c$16$1$123 ==.
                                   1479 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:16: volatile unsigned char relogio[QT_TEMPO] = {0,0,0,0,0,0,0};
                                   1480 ;	1-genFromRTrack replaced	mov	_relogio,#0x00
      000092 F5 2E            [12] 1481 	mov	_relogio,a
                                   1482 ;	1-genFromRTrack replaced	mov	(_relogio + 0x0001),#0x00
      000094 F5 2F            [12] 1483 	mov	(_relogio + 0x0001),a
                                   1484 ;	1-genFromRTrack replaced	mov	(_relogio + 0x0002),#0x00
      000096 F5 30            [12] 1485 	mov	(_relogio + 0x0002),a
                                   1486 ;	1-genFromRTrack replaced	mov	(_relogio + 0x0003),#0x00
      000098 F5 31            [12] 1487 	mov	(_relogio + 0x0003),a
                                   1488 ;	1-genFromRTrack replaced	mov	(_relogio + 0x0004),#0x00
      00009A F5 32            [12] 1489 	mov	(_relogio + 0x0004),a
                                   1490 ;	1-genFromRTrack replaced	mov	(_relogio + 0x0005),#0x00
      00009C F5 33            [12] 1491 	mov	(_relogio + 0x0005),a
                                   1492 ;	1-genFromRTrack replaced	mov	(_relogio + 0x0006),#0x00
      00009E F5 34            [12] 1493 	mov	(_relogio + 0x0006),a
                           000016  1494 	C$main.c$17$1$123 ==.
                                   1495 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:17: volatile unsigned char tecla = 0;
                                   1496 ;	1-genFromRTrack replaced	mov	_tecla,#0x00
      0000A0 F5 47            [12] 1497 	mov	_tecla,a
                           000018  1498 	C$glcd.c$22$1$123 ==.
                                   1499 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:22: volatile __bit terminal_ativo = 0;
      0000A2 C2 00            [12] 1500 	clr	_terminal_ativo
                           00001A  1501 	C$sensores.c$36$1$123 ==.
                                   1502 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:36: volatile __bit transmissao_dht11=0;
      0000A4 C2 0B            [12] 1503 	clr	_transmissao_dht11
                           00001C  1504 	C$main.c$16$1$123 ==.
                                   1505 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:16: volatile __bit flag_tecla = 0;
      0000A6 C2 0C            [12] 1506 	clr	_flag_tecla
                                   1507 	.area GSFINAL (CODE)
      0000A8 02 00 2E         [24] 1508 	ljmp	__sdcc_program_startup
                                   1509 ;--------------------------------------------------------
                                   1510 ; Home
                                   1511 ;--------------------------------------------------------
                                   1512 	.area HOME    (CODE)
                                   1513 	.area HOME    (CODE)
      00002E                       1514 __sdcc_program_startup:
      00002E 02 0D B6         [24] 1515 	ljmp	_main
                                   1516 ;	return from main will return to caller
                                   1517 ;--------------------------------------------------------
                                   1518 ; code
                                   1519 ;--------------------------------------------------------
                                   1520 	.area CSEG    (CODE)
                                   1521 ;------------------------------------------------------------
                                   1522 ;Allocation info for local variables in function 'Reset_Sources_Init'
                                   1523 ;------------------------------------------------------------
                           000000  1524 	G$Reset_Sources_Init$0$0 ==.
                           000000  1525 	C$config.c$10$0$0 ==.
                                   1526 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:10: void Reset_Sources_Init()
                                   1527 ;	-----------------------------------------
                                   1528 ;	 function Reset_Sources_Init
                                   1529 ;	-----------------------------------------
      0000AB                       1530 _Reset_Sources_Init:
                           000007  1531 	ar7 = 0x07
                           000006  1532 	ar6 = 0x06
                           000005  1533 	ar5 = 0x05
                           000004  1534 	ar4 = 0x04
                           000003  1535 	ar3 = 0x03
                           000002  1536 	ar2 = 0x02
                           000001  1537 	ar1 = 0x01
                           000000  1538 	ar0 = 0x00
                           000000  1539 	C$config.c$12$1$14 ==.
                                   1540 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:12: WDTCN     = 0xDE;
      0000AB 75 FF DE         [24] 1541 	mov	_WDTCN,#0xde
                           000003  1542 	C$config.c$13$1$14 ==.
                                   1543 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:13: WDTCN     = 0xAD;
      0000AE 75 FF AD         [24] 1544 	mov	_WDTCN,#0xad
                           000006  1545 	C$config.c$14$1$14 ==.
                           000006  1546 	XG$Reset_Sources_Init$0$0 ==.
      0000B1 22               [24] 1547 	ret
                                   1548 ;------------------------------------------------------------
                                   1549 ;Allocation info for local variables in function 'Timer_Init'
                                   1550 ;------------------------------------------------------------
                           000007  1551 	G$Timer_Init$0$0 ==.
                           000007  1552 	C$config.c$16$1$14 ==.
                                   1553 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:16: void Timer_Init()
                                   1554 ;	-----------------------------------------
                                   1555 ;	 function Timer_Init
                                   1556 ;	-----------------------------------------
      0000B2                       1557 _Timer_Init:
                           000007  1558 	C$config.c$18$1$15 ==.
                                   1559 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:18: SFRPAGE   = TIMER01_PAGE;
      0000B2 75 84 00         [24] 1560 	mov	_SFRPAGE,#0x00
                           00000A  1561 	C$config.c$19$1$15 ==.
                                   1562 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:19: TCON      = 0x40;
      0000B5 75 88 40         [24] 1563 	mov	_TCON,#0x40
                           00000D  1564 	C$config.c$20$1$15 ==.
                                   1565 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:20: TMOD      = 0x21;
      0000B8 75 89 21         [24] 1566 	mov	_TMOD,#0x21
                           000010  1567 	C$config.c$21$1$15 ==.
                                   1568 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:21: CKCON     = 0x18;
      0000BB 75 8E 18         [24] 1569 	mov	_CKCON,#0x18
                           000013  1570 	C$config.c$22$1$15 ==.
                                   1571 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:22: TH1       = 0xAF;
      0000BE 75 8D AF         [24] 1572 	mov	_TH1,#0xaf
                           000016  1573 	C$config.c$23$1$15 ==.
                                   1574 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:23: SFRPAGE   = TMR2_PAGE;
      0000C1 75 84 00         [24] 1575 	mov	_SFRPAGE,#0x00
                           000019  1576 	C$config.c$24$1$15 ==.
                                   1577 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:24: TMR2CN    = 0x04;
      0000C4 75 C8 04         [24] 1578 	mov	_TMR2CN,#0x04
                           00001C  1579 	C$config.c$25$1$15 ==.
                                   1580 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:25: TMR2CF    = 0x18;
      0000C7 75 C9 18         [24] 1581 	mov	_TMR2CF,#0x18
                           00001F  1582 	C$config.c$26$1$15 ==.
                                   1583 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:26: RCAP2L    = 0xDC;
      0000CA 75 CA DC         [24] 1584 	mov	_RCAP2L,#0xdc
                           000022  1585 	C$config.c$27$1$15 ==.
                                   1586 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:27: RCAP2H    = 0x0B;
      0000CD 75 CB 0B         [24] 1587 	mov	_RCAP2H,#0x0b
                           000025  1588 	C$config.c$28$1$15 ==.
                                   1589 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:28: TMR2L     = 0xDC;
      0000D0 75 CC DC         [24] 1590 	mov	_TMR2L,#0xdc
                           000028  1591 	C$config.c$29$1$15 ==.
                                   1592 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:29: TMR2H     = 0x0B;
      0000D3 75 CD 0B         [24] 1593 	mov	_TMR2H,#0x0b
                           00002B  1594 	C$config.c$30$1$15 ==.
                                   1595 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:30: SFRPAGE   = TMR4_PAGE;
      0000D6 75 84 02         [24] 1596 	mov	_SFRPAGE,#0x02
                           00002E  1597 	C$config.c$31$1$15 ==.
                                   1598 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:31: TMR4CN    = 0x04;
      0000D9 75 C8 04         [24] 1599 	mov	_TMR4CN,#0x04
                           000031  1600 	C$config.c$32$1$15 ==.
                                   1601 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:32: TMR4CF    = 0x02;
      0000DC 75 C9 02         [24] 1602 	mov	_TMR4CF,#0x02
                           000034  1603 	C$config.c$33$1$15 ==.
                                   1604 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:33: RCAP4L    = 0x8D;
      0000DF 75 CA 8D         [24] 1605 	mov	_RCAP4L,#0x8d
                           000037  1606 	C$config.c$34$1$15 ==.
                                   1607 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:34: RCAP4H    = 0x34;
      0000E2 75 CB 34         [24] 1608 	mov	_RCAP4H,#0x34
                           00003A  1609 	C$config.c$35$1$15 ==.
                           00003A  1610 	XG$Timer_Init$0$0 ==.
      0000E5 22               [24] 1611 	ret
                                   1612 ;------------------------------------------------------------
                                   1613 ;Allocation info for local variables in function 'UART_Init'
                                   1614 ;------------------------------------------------------------
                           00003B  1615 	G$UART_Init$0$0 ==.
                           00003B  1616 	C$config.c$37$1$15 ==.
                                   1617 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:37: void UART_Init()
                                   1618 ;	-----------------------------------------
                                   1619 ;	 function UART_Init
                                   1620 ;	-----------------------------------------
      0000E6                       1621 _UART_Init:
                           00003B  1622 	C$config.c$39$1$16 ==.
                                   1623 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:39: SFRPAGE   = UART0_PAGE;
      0000E6 75 84 00         [24] 1624 	mov	_SFRPAGE,#0x00
                           00003E  1625 	C$config.c$40$1$16 ==.
                                   1626 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:40: SCON0     = 0x70;
      0000E9 75 98 70         [24] 1627 	mov	_SCON0,#0x70
                           000041  1628 	C$config.c$41$1$16 ==.
                           000041  1629 	XG$UART_Init$0$0 ==.
      0000EC 22               [24] 1630 	ret
                                   1631 ;------------------------------------------------------------
                                   1632 ;Allocation info for local variables in function 'SMBus_Init'
                                   1633 ;------------------------------------------------------------
                           000042  1634 	G$SMBus_Init$0$0 ==.
                           000042  1635 	C$config.c$43$1$16 ==.
                                   1636 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:43: void SMBus_Init()
                                   1637 ;	-----------------------------------------
                                   1638 ;	 function SMBus_Init
                                   1639 ;	-----------------------------------------
      0000ED                       1640 _SMBus_Init:
                           000042  1641 	C$config.c$45$1$17 ==.
                                   1642 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:45: SFRPAGE   = SMB0_PAGE;
      0000ED 75 84 00         [24] 1643 	mov	_SFRPAGE,#0x00
                           000045  1644 	C$config.c$46$1$17 ==.
                                   1645 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:46: SMB0CR    = 0xE9;
      0000F0 75 CF E9         [24] 1646 	mov	_SMB0CR,#0xe9
                           000048  1647 	C$config.c$47$1$17 ==.
                           000048  1648 	XG$SMBus_Init$0$0 ==.
      0000F3 22               [24] 1649 	ret
                                   1650 ;------------------------------------------------------------
                                   1651 ;Allocation info for local variables in function 'SPI_Init'
                                   1652 ;------------------------------------------------------------
                           000049  1653 	G$SPI_Init$0$0 ==.
                           000049  1654 	C$config.c$49$1$17 ==.
                                   1655 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:49: void SPI_Init()
                                   1656 ;	-----------------------------------------
                                   1657 ;	 function SPI_Init
                                   1658 ;	-----------------------------------------
      0000F4                       1659 _SPI_Init:
                           000049  1660 	C$config.c$51$1$18 ==.
                                   1661 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:51: SFRPAGE   = SPI0_PAGE;
      0000F4 75 84 00         [24] 1662 	mov	_SFRPAGE,#0x00
                           00004C  1663 	C$config.c$52$1$18 ==.
                                   1664 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:52: SPI0CFG   = 0x40;
      0000F7 75 9A 40         [24] 1665 	mov	_SPI0CFG,#0x40
                           00004F  1666 	C$config.c$53$1$18 ==.
                                   1667 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:53: SPI0CN    = 0x01;
      0000FA 75 F8 01         [24] 1668 	mov	_SPI0CN,#0x01
                           000052  1669 	C$config.c$54$1$18 ==.
                                   1670 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:54: SPI0CKR   = 0x7C;
      0000FD 75 9D 7C         [24] 1671 	mov	_SPI0CKR,#0x7c
                           000055  1672 	C$config.c$55$1$18 ==.
                           000055  1673 	XG$SPI_Init$0$0 ==.
      000100 22               [24] 1674 	ret
                                   1675 ;------------------------------------------------------------
                                   1676 ;Allocation info for local variables in function 'ADC_Init'
                                   1677 ;------------------------------------------------------------
                           000056  1678 	G$ADC_Init$0$0 ==.
                           000056  1679 	C$config.c$57$1$18 ==.
                                   1680 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:57: void ADC_Init()
                                   1681 ;	-----------------------------------------
                                   1682 ;	 function ADC_Init
                                   1683 ;	-----------------------------------------
      000101                       1684 _ADC_Init:
                           000056  1685 	C$config.c$59$1$19 ==.
                                   1686 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:59: SFRPAGE   = ADC0_PAGE;
      000101 75 84 00         [24] 1687 	mov	_SFRPAGE,#0x00
                           000059  1688 	C$config.c$60$1$19 ==.
                                   1689 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:60: ADC0CN    = 0x80;
      000104 75 E8 80         [24] 1690 	mov	_ADC0CN,#0x80
                           00005C  1691 	C$config.c$61$1$19 ==.
                           00005C  1692 	XG$ADC_Init$0$0 ==.
      000107 22               [24] 1693 	ret
                                   1694 ;------------------------------------------------------------
                                   1695 ;Allocation info for local variables in function 'DAC_Init'
                                   1696 ;------------------------------------------------------------
                           00005D  1697 	G$DAC_Init$0$0 ==.
                           00005D  1698 	C$config.c$63$1$19 ==.
                                   1699 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:63: void DAC_Init()
                                   1700 ;	-----------------------------------------
                                   1701 ;	 function DAC_Init
                                   1702 ;	-----------------------------------------
      000108                       1703 _DAC_Init:
                           00005D  1704 	C$config.c$65$1$20 ==.
                                   1705 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:65: SFRPAGE   = DAC0_PAGE;
      000108 75 84 00         [24] 1706 	mov	_SFRPAGE,#0x00
                           000060  1707 	C$config.c$66$1$20 ==.
                                   1708 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:66: DAC0CN    = 0x9C;
      00010B 75 D4 9C         [24] 1709 	mov	_DAC0CN,#0x9c
                           000063  1710 	C$config.c$67$1$20 ==.
                           000063  1711 	XG$DAC_Init$0$0 ==.
      00010E 22               [24] 1712 	ret
                                   1713 ;------------------------------------------------------------
                                   1714 ;Allocation info for local variables in function 'Voltage_Reference_Init'
                                   1715 ;------------------------------------------------------------
                           000064  1716 	G$Voltage_Reference_Init$0$0 ==.
                           000064  1717 	C$config.c$69$1$20 ==.
                                   1718 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:69: void Voltage_Reference_Init()
                                   1719 ;	-----------------------------------------
                                   1720 ;	 function Voltage_Reference_Init
                                   1721 ;	-----------------------------------------
      00010F                       1722 _Voltage_Reference_Init:
                           000064  1723 	C$config.c$71$1$21 ==.
                                   1724 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:71: SFRPAGE   = ADC0_PAGE;
      00010F 75 84 00         [24] 1725 	mov	_SFRPAGE,#0x00
                           000067  1726 	C$config.c$72$1$21 ==.
                                   1727 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:72: REF0CN    = 0x03;
      000112 75 D1 03         [24] 1728 	mov	_REF0CN,#0x03
                           00006A  1729 	C$config.c$73$1$21 ==.
                           00006A  1730 	XG$Voltage_Reference_Init$0$0 ==.
      000115 22               [24] 1731 	ret
                                   1732 ;------------------------------------------------------------
                                   1733 ;Allocation info for local variables in function 'Port_IO_Init'
                                   1734 ;------------------------------------------------------------
                           00006B  1735 	G$Port_IO_Init$0$0 ==.
                           00006B  1736 	C$config.c$75$1$21 ==.
                                   1737 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:75: void Port_IO_Init()
                                   1738 ;	-----------------------------------------
                                   1739 ;	 function Port_IO_Init
                                   1740 ;	-----------------------------------------
      000116                       1741 _Port_IO_Init:
                           00006B  1742 	C$config.c$113$1$22 ==.
                                   1743 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:113: SFRPAGE   = CONFIG_PAGE;
      000116 75 84 0F         [24] 1744 	mov	_SFRPAGE,#0x0f
                           00006E  1745 	C$config.c$114$1$22 ==.
                                   1746 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:114: P0MDOUT   = 0x15;
      000119 75 A4 15         [24] 1747 	mov	_P0MDOUT,#0x15
                           000071  1748 	C$config.c$115$1$22 ==.
                                   1749 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:115: P2MDOUT   = 0xFF;
      00011C 75 A6 FF         [24] 1750 	mov	_P2MDOUT,#0xff
                           000074  1751 	C$config.c$116$1$22 ==.
                                   1752 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:116: P3MDOUT   = 0xFF;
      00011F 75 A7 FF         [24] 1753 	mov	_P3MDOUT,#0xff
                           000077  1754 	C$config.c$117$1$22 ==.
                                   1755 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:117: XBR0      = 0x06;
      000122 75 E1 06         [24] 1756 	mov	_XBR0,#0x06
                           00007A  1757 	C$config.c$118$1$22 ==.
                                   1758 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:118: XBR2      = 0x40;
      000125 75 E3 40         [24] 1759 	mov	_XBR2,#0x40
                           00007D  1760 	C$config.c$119$1$22 ==.
                           00007D  1761 	XG$Port_IO_Init$0$0 ==.
      000128 22               [24] 1762 	ret
                                   1763 ;------------------------------------------------------------
                                   1764 ;Allocation info for local variables in function 'Oscillator_Init'
                                   1765 ;------------------------------------------------------------
                                   1766 ;i                         Allocated to registers r6 r7 
                                   1767 ;------------------------------------------------------------
                           00007E  1768 	G$Oscillator_Init$0$0 ==.
                           00007E  1769 	C$config.c$121$1$22 ==.
                                   1770 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:121: void Oscillator_Init()
                                   1771 ;	-----------------------------------------
                                   1772 ;	 function Oscillator_Init
                                   1773 ;	-----------------------------------------
      000129                       1774 _Oscillator_Init:
                           00007E  1775 	C$config.c$124$1$23 ==.
                                   1776 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:124: SFRPAGE   = CONFIG_PAGE;
      000129 75 84 0F         [24] 1777 	mov	_SFRPAGE,#0x0f
                           000081  1778 	C$config.c$125$1$23 ==.
                                   1779 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:125: OSCXCN    = 0x67;
      00012C 75 8C 67         [24] 1780 	mov	_OSCXCN,#0x67
                           000084  1781 	C$config.c$126$1$23 ==.
                                   1782 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:126: for (i = 0; i < 3000; i++);  // Wait 1ms for initialization
      00012F 7E B8            [12] 1783 	mov	r6,#0xb8
      000131 7F 0B            [12] 1784 	mov	r7,#0x0b
      000133                       1785 00107$:
      000133 EE               [12] 1786 	mov	a,r6
      000134 24 FF            [12] 1787 	add	a,#0xff
      000136 FC               [12] 1788 	mov	r4,a
      000137 EF               [12] 1789 	mov	a,r7
      000138 34 FF            [12] 1790 	addc	a,#0xff
      00013A FD               [12] 1791 	mov	r5,a
      00013B 8C 06            [24] 1792 	mov	ar6,r4
      00013D 8D 07            [24] 1793 	mov	ar7,r5
      00013F EC               [12] 1794 	mov	a,r4
      000140 4D               [12] 1795 	orl	a,r5
      000141 70 F0            [24] 1796 	jnz	00107$
                           000098  1797 	C$config.c$127$1$23 ==.
                                   1798 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:127: while ((OSCXCN & 0x80) == 0);
      000143                       1799 00102$:
      000143 E5 8C            [12] 1800 	mov	a,_OSCXCN
      000145 30 E7 FB         [24] 1801 	jnb	acc.7,00102$
                           00009D  1802 	C$config.c$128$1$23 ==.
                                   1803 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:128: CLKSEL    = 0x01;
      000148 75 97 01         [24] 1804 	mov	_CLKSEL,#0x01
                           0000A0  1805 	C$config.c$129$1$23 ==.
                           0000A0  1806 	XG$Oscillator_Init$0$0 ==.
      00014B 22               [24] 1807 	ret
                                   1808 ;------------------------------------------------------------
                                   1809 ;Allocation info for local variables in function 'Interrupts_Init'
                                   1810 ;------------------------------------------------------------
                           0000A1  1811 	G$Interrupts_Init$0$0 ==.
                           0000A1  1812 	C$config.c$131$1$23 ==.
                                   1813 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:131: void Interrupts_Init()
                                   1814 ;	-----------------------------------------
                                   1815 ;	 function Interrupts_Init
                                   1816 ;	-----------------------------------------
      00014C                       1817 _Interrupts_Init:
                           0000A1  1818 	C$config.c$133$1$24 ==.
                                   1819 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:133: IE        = 0xB0;
      00014C 75 A8 B0         [24] 1820 	mov	_IE,#0xb0
                           0000A4  1821 	C$config.c$134$1$24 ==.
                           0000A4  1822 	XG$Interrupts_Init$0$0 ==.
      00014F 22               [24] 1823 	ret
                                   1824 ;------------------------------------------------------------
                                   1825 ;Allocation info for local variables in function 'Init_Device'
                                   1826 ;------------------------------------------------------------
                           0000A5  1827 	G$Init_Device$0$0 ==.
                           0000A5  1828 	C$config.c$138$1$24 ==.
                                   1829 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:138: void Init_Device(void)
                                   1830 ;	-----------------------------------------
                                   1831 ;	 function Init_Device
                                   1832 ;	-----------------------------------------
      000150                       1833 _Init_Device:
                           0000A5  1834 	C$config.c$140$1$26 ==.
                                   1835 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:140: Reset_Sources_Init();
      000150 12 00 AB         [24] 1836 	lcall	_Reset_Sources_Init
                           0000A8  1837 	C$config.c$141$1$26 ==.
                                   1838 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:141: Timer_Init();
      000153 12 00 B2         [24] 1839 	lcall	_Timer_Init
                           0000AB  1840 	C$config.c$142$1$26 ==.
                                   1841 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:142: UART_Init();
      000156 12 00 E6         [24] 1842 	lcall	_UART_Init
                           0000AE  1843 	C$config.c$143$1$26 ==.
                                   1844 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:143: SMBus_Init();
      000159 12 00 ED         [24] 1845 	lcall	_SMBus_Init
                           0000B1  1846 	C$config.c$144$1$26 ==.
                                   1847 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:144: SPI_Init();
      00015C 12 00 F4         [24] 1848 	lcall	_SPI_Init
                           0000B4  1849 	C$config.c$145$1$26 ==.
                                   1850 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:145: ADC_Init();
      00015F 12 01 01         [24] 1851 	lcall	_ADC_Init
                           0000B7  1852 	C$config.c$146$1$26 ==.
                                   1853 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:146: DAC_Init();
      000162 12 01 08         [24] 1854 	lcall	_DAC_Init
                           0000BA  1855 	C$config.c$147$1$26 ==.
                                   1856 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:147: Voltage_Reference_Init();
      000165 12 01 0F         [24] 1857 	lcall	_Voltage_Reference_Init
                           0000BD  1858 	C$config.c$148$1$26 ==.
                                   1859 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:148: Port_IO_Init();
      000168 12 01 16         [24] 1860 	lcall	_Port_IO_Init
                           0000C0  1861 	C$config.c$149$1$26 ==.
                                   1862 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:149: Oscillator_Init();
      00016B 12 01 29         [24] 1863 	lcall	_Oscillator_Init
                           0000C3  1864 	C$config.c$150$1$26 ==.
                                   1865 ;	C:\Users\202019050584\Desktop\Trabalho\/config.c:150: Interrupts_Init();
      00016E 12 01 4C         [24] 1866 	lcall	_Interrupts_Init
                           0000C6  1867 	C$config.c$151$1$26 ==.
                           0000C6  1868 	XG$Init_Device$0$0 ==.
      000171 22               [24] 1869 	ret
                                   1870 ;------------------------------------------------------------
                                   1871 ;Allocation info for local variables in function 'le_glcd'
                                   1872 ;------------------------------------------------------------
                                   1873 ;byte                      Allocated to registers 
                                   1874 ;------------------------------------------------------------
                           0000C7  1875 	G$le_glcd$0$0 ==.
                           0000C7  1876 	C$glcd.c$125$1$26 ==.
                                   1877 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:125: unsigned char le_glcd(__bit cd, __bit cs){
                                   1878 ;	-----------------------------------------
                                   1879 ;	 function le_glcd
                                   1880 ;	-----------------------------------------
      000172                       1881 _le_glcd:
                           0000C7  1882 	C$glcd.c$130$1$28 ==.
                                   1883 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:130: RW = HI;
      000172 D2 A3            [12] 1884 	setb	_P2_3
                           0000C9  1885 	C$glcd.c$131$1$28 ==.
                                   1886 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:131: CS1 = cs;
      000174 A2 02            [12] 1887 	mov	c,_le_glcd_PARM_2
      000176 92 A0            [24] 1888 	mov	_P2_0,c
                           0000CD  1889 	C$glcd.c$132$1$28 ==.
                                   1890 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:132: CS2 = !cs;
      000178 A2 02            [12] 1891 	mov	c,_le_glcd_PARM_2
      00017A B3               [12] 1892 	cpl	c
      00017B 92 A1            [24] 1893 	mov	_P2_1,c
                           0000D2  1894 	C$glcd.c$133$1$28 ==.
                                   1895 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:133: RS = cd;
      00017D A2 01            [12] 1896 	mov	c,_le_glcd_PARM_1
      00017F 92 A2            [24] 1897 	mov	_P2_2,c
                           0000D6  1898 	C$glcd.c$134$1$28 ==.
                                   1899 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:134: NOP4();
      000181 00               [12] 1900 	NOP	
      000182 00               [12] 1901 	NOP	
      000183 00               [12] 1902 	NOP	
      000184 00               [12] 1903 	NOP	
                           0000DA  1904 	C$glcd.c$136$1$28 ==.
                                   1905 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:136: E = HI;
      000185 D2 A4            [12] 1906 	setb	_P2_4
                           0000DC  1907 	C$glcd.c$137$1$28 ==.
                                   1908 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:137: NOP8();
      000187 00               [12] 1909 	NOP	
      000188 00               [12] 1910 	NOP	
      000189 00               [12] 1911 	NOP	
      00018A 00               [12] 1912 	NOP	
      00018B 00               [12] 1913 	NOP	
      00018C 00               [12] 1914 	NOP	
      00018D 00               [12] 1915 	NOP	
      00018E 00               [12] 1916 	NOP	
                           0000E4  1917 	C$glcd.c$139$1$28 ==.
                                   1918 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:139: SFRPAGE=CONFIG_PAGE;
      00018F 75 84 0F         [24] 1919 	mov	_SFRPAGE,#0x0f
                           0000E7  1920 	C$glcd.c$140$1$28 ==.
                                   1921 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:140: byte = DB;
      000192 85 C8 82         [24] 1922 	mov	dpl,_P4
                           0000EA  1923 	C$glcd.c$141$1$28 ==.
                                   1924 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:141: SFRPAGE=LEGACY_PAGE;
      000195 75 84 00         [24] 1925 	mov	_SFRPAGE,#0x00
                           0000ED  1926 	C$glcd.c$142$1$28 ==.
                                   1927 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:142: NOP4();
      000198 00               [12] 1928 	NOP	
      000199 00               [12] 1929 	NOP	
      00019A 00               [12] 1930 	NOP	
      00019B 00               [12] 1931 	NOP	
                           0000F1  1932 	C$glcd.c$144$1$28 ==.
                                   1933 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:144: E = LO;
      00019C C2 A4            [12] 1934 	clr	_P2_4
                           0000F3  1935 	C$glcd.c$145$1$28 ==.
                                   1936 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:145: NOP12();
      00019E 00               [12] 1937 	NOP	
      00019F 00               [12] 1938 	NOP	
      0001A0 00               [12] 1939 	NOP	
      0001A1 00               [12] 1940 	NOP	
      0001A2 00               [12] 1941 	NOP	
      0001A3 00               [12] 1942 	NOP	
      0001A4 00               [12] 1943 	NOP	
      0001A5 00               [12] 1944 	NOP	
      0001A6 00               [12] 1945 	NOP	
      0001A7 00               [12] 1946 	NOP	
      0001A8 00               [12] 1947 	NOP	
      0001A9 00               [12] 1948 	NOP	
                           0000FF  1949 	C$glcd.c$146$1$28 ==.
                                   1950 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:146: return (byte);
                           0000FF  1951 	C$glcd.c$148$1$28 ==.
                           0000FF  1952 	XG$le_glcd$0$0 ==.
      0001AA 22               [24] 1953 	ret
                                   1954 ;------------------------------------------------------------
                                   1955 ;Allocation info for local variables in function 'esc_glcd'
                                   1956 ;------------------------------------------------------------
                                   1957 ;byte                      Allocated to registers r7 
                                   1958 ;------------------------------------------------------------
                           000100  1959 	G$esc_glcd$0$0 ==.
                           000100  1960 	C$glcd.c$150$1$28 ==.
                                   1961 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:150: void esc_glcd(unsigned char byte, __bit cd, __bit cs){
                                   1962 ;	-----------------------------------------
                                   1963 ;	 function esc_glcd
                                   1964 ;	-----------------------------------------
      0001AB                       1965 _esc_glcd:
      0001AB AF 82            [24] 1966 	mov	r7,dpl
                           000102  1967 	C$glcd.c$153$1$30 ==.
                                   1968 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:153: while(le_glcd(CO, cs) & 0x80); // Espera enquanto BUSY for 1
      0001AD                       1969 00101$:
      0001AD C2 01            [12] 1970 	clr	_le_glcd_PARM_1
      0001AF A2 04            [12] 1971 	mov	c,_esc_glcd_PARM_3
      0001B1 92 02            [24] 1972 	mov	_le_glcd_PARM_2,c
      0001B3 C0 07            [24] 1973 	push	ar7
      0001B5 12 01 72         [24] 1974 	lcall	_le_glcd
      0001B8 E5 82            [12] 1975 	mov	a,dpl
      0001BA D0 07            [24] 1976 	pop	ar7
      0001BC 20 E7 EE         [24] 1977 	jb	acc.7,00101$
                           000114  1978 	C$glcd.c$155$1$30 ==.
                                   1979 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:155: RW = LO;
      0001BF C2 A3            [12] 1980 	clr	_P2_3
                           000116  1981 	C$glcd.c$156$1$30 ==.
                                   1982 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:156: CS1 = cs;
      0001C1 A2 04            [12] 1983 	mov	c,_esc_glcd_PARM_3
      0001C3 92 A0            [24] 1984 	mov	_P2_0,c
                           00011A  1985 	C$glcd.c$157$1$30 ==.
                                   1986 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:157: CS2 = !cs;
      0001C5 A2 04            [12] 1987 	mov	c,_esc_glcd_PARM_3
      0001C7 B3               [12] 1988 	cpl	c
      0001C8 92 A1            [24] 1989 	mov	_P2_1,c
                           00011F  1990 	C$glcd.c$158$1$30 ==.
                                   1991 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:158: RS = cd;
      0001CA A2 03            [12] 1992 	mov	c,_esc_glcd_PARM_2
      0001CC 92 A2            [24] 1993 	mov	_P2_2,c
                           000123  1994 	C$glcd.c$159$1$30 ==.
                                   1995 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:159: SFRPAGE=CONFIG_PAGE;
      0001CE 75 84 0F         [24] 1996 	mov	_SFRPAGE,#0x0f
                           000126  1997 	C$glcd.c$160$1$30 ==.
                                   1998 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:160: DB = byte;
      0001D1 8F C8            [24] 1999 	mov	_P4,r7
                           000128  2000 	C$glcd.c$161$1$30 ==.
                                   2001 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:161: SFRPAGE=LEGACY_PAGE;
      0001D3 75 84 00         [24] 2002 	mov	_SFRPAGE,#0x00
                           00012B  2003 	C$glcd.c$162$1$30 ==.
                                   2004 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:162: NOP4();
      0001D6 00               [12] 2005 	NOP	
      0001D7 00               [12] 2006 	NOP	
      0001D8 00               [12] 2007 	NOP	
      0001D9 00               [12] 2008 	NOP	
                           00012F  2009 	C$glcd.c$164$1$30 ==.
                                   2010 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:164: E = HI;
      0001DA D2 A4            [12] 2011 	setb	_P2_4
                           000131  2012 	C$glcd.c$165$1$30 ==.
                                   2013 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:165: NOP12();
      0001DC 00               [12] 2014 	NOP	
      0001DD 00               [12] 2015 	NOP	
      0001DE 00               [12] 2016 	NOP	
      0001DF 00               [12] 2017 	NOP	
      0001E0 00               [12] 2018 	NOP	
      0001E1 00               [12] 2019 	NOP	
      0001E2 00               [12] 2020 	NOP	
      0001E3 00               [12] 2021 	NOP	
      0001E4 00               [12] 2022 	NOP	
      0001E5 00               [12] 2023 	NOP	
      0001E6 00               [12] 2024 	NOP	
      0001E7 00               [12] 2025 	NOP	
                           00013D  2026 	C$glcd.c$167$1$30 ==.
                                   2027 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:167: E = LO;
      0001E8 C2 A4            [12] 2028 	clr	_P2_4
                           00013F  2029 	C$glcd.c$168$1$30 ==.
                                   2030 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:168: SFRPAGE=CONFIG_PAGE;
      0001EA 75 84 0F         [24] 2031 	mov	_SFRPAGE,#0x0f
                           000142  2032 	C$glcd.c$169$1$30 ==.
                                   2033 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:169: DB = 0xff; // Para que a porta funcione como um entrada de novo sem nenhum problema
      0001ED 75 C8 FF         [24] 2034 	mov	_P4,#0xff
                           000145  2035 	C$glcd.c$170$1$30 ==.
                                   2036 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:170: SFRPAGE=LEGACY_PAGE;
      0001F0 75 84 00         [24] 2037 	mov	_SFRPAGE,#0x00
                           000148  2038 	C$glcd.c$171$1$30 ==.
                                   2039 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:171: RW = HI; // RW == P2_3 sao usados pelo GLCD e precisa ser setado 1 para ser usado por outra funcao de outro componente
      0001F3 D2 A3            [12] 2040 	setb	_P2_3
                           00014A  2041 	C$glcd.c$172$1$30 ==.
                                   2042 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:172: NOP12();
      0001F5 00               [12] 2043 	NOP	
      0001F6 00               [12] 2044 	NOP	
      0001F7 00               [12] 2045 	NOP	
      0001F8 00               [12] 2046 	NOP	
      0001F9 00               [12] 2047 	NOP	
      0001FA 00               [12] 2048 	NOP	
      0001FB 00               [12] 2049 	NOP	
      0001FC 00               [12] 2050 	NOP	
      0001FD 00               [12] 2051 	NOP	
      0001FE 00               [12] 2052 	NOP	
      0001FF 00               [12] 2053 	NOP	
      000200 00               [12] 2054 	NOP	
                           000156  2055 	C$glcd.c$173$1$30 ==.
                           000156  2056 	XG$esc_glcd$0$0 ==.
      000201 22               [24] 2057 	ret
                                   2058 ;------------------------------------------------------------
                                   2059 ;Allocation info for local variables in function 'ini_glcd'
                                   2060 ;------------------------------------------------------------
                                   2061 ;cs                        Allocated to registers r7 
                                   2062 ;------------------------------------------------------------
                           000157  2063 	G$ini_glcd$0$0 ==.
                           000157  2064 	C$glcd.c$175$1$30 ==.
                                   2065 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:175: void ini_glcd(){
                                   2066 ;	-----------------------------------------
                                   2067 ;	 function ini_glcd
                                   2068 ;	-----------------------------------------
      000202                       2069 _ini_glcd:
                           000157  2070 	C$glcd.c$180$1$31 ==.
                                   2071 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:180: E = LO;
      000202 C2 A4            [12] 2072 	clr	_P2_4
                           000159  2073 	C$glcd.c$181$1$31 ==.
                                   2074 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:181: RST = HI;
      000204 D2 A5            [12] 2075 	setb	_P2_5
                           00015B  2076 	C$glcd.c$182$1$31 ==.
                                   2077 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:182: CS1 = HI;
      000206 D2 A0            [12] 2078 	setb	_P2_0
                           00015D  2079 	C$glcd.c$183$1$31 ==.
                                   2080 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:183: CS2 = HI;
      000208 D2 A1            [12] 2081 	setb	_P2_1
                           00015F  2082 	C$glcd.c$184$1$31 ==.
                                   2083 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:184: SFRPAGE=CONFIG_PAGE;
      00020A 75 84 0F         [24] 2084 	mov	_SFRPAGE,#0x0f
                           000162  2085 	C$glcd.c$185$1$31 ==.
                                   2086 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:185: DB = 0xff;
      00020D 75 C8 FF         [24] 2087 	mov	_P4,#0xff
                           000165  2088 	C$glcd.c$186$1$31 ==.
                                   2089 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:186: SFRPAGE=LEGACY_PAGE;
      000210 75 84 00         [24] 2090 	mov	_SFRPAGE,#0x00
                           000168  2091 	C$glcd.c$188$1$31 ==.
                                   2092 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:188: while(cs<2){
      000213 7F 00            [12] 2093 	mov	r7,#0x00
      000215                       2094 00104$:
      000215 BF 02 00         [24] 2095 	cjne	r7,#0x02,00119$
      000218                       2096 00119$:
      000218 50 4E            [24] 2097 	jnc	00107$
                           00016F  2098 	C$glcd.c$190$2$32 ==.
                                   2099 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:190: while(le_glcd(CO, cs) & 0x10);
      00021A                       2100 00101$:
      00021A EF               [12] 2101 	mov	a,r7
      00021B 24 FF            [12] 2102 	add	a,#0xff
      00021D 92 05            [24] 2103 	mov	_ini_glcd_sloc0_1_0,c
      00021F C2 01            [12] 2104 	clr	_le_glcd_PARM_1
      000221 A2 05            [12] 2105 	mov	c,_ini_glcd_sloc0_1_0
      000223 92 02            [24] 2106 	mov	_le_glcd_PARM_2,c
      000225 C0 07            [24] 2107 	push	ar7
      000227 12 01 72         [24] 2108 	lcall	_le_glcd
      00022A E5 82            [12] 2109 	mov	a,dpl
      00022C D0 07            [24] 2110 	pop	ar7
      00022E 20 E4 E9         [24] 2111 	jb	acc.4,00101$
                           000186  2112 	C$glcd.c$193$2$32 ==.
                                   2113 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:193: esc_glcd(0x3f, CO, cs);
      000231 C2 03            [12] 2114 	clr	_esc_glcd_PARM_2
      000233 A2 05            [12] 2115 	mov	c,_ini_glcd_sloc0_1_0
      000235 92 04            [24] 2116 	mov	_esc_glcd_PARM_3,c
      000237 75 82 3F         [24] 2117 	mov	dpl,#0x3f
      00023A C0 07            [24] 2118 	push	ar7
      00023C 12 01 AB         [24] 2119 	lcall	_esc_glcd
                           000194  2120 	C$glcd.c$196$2$32 ==.
                                   2121 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:196: esc_glcd(0x40, CO, cs); // Y
      00023F C2 03            [12] 2122 	clr	_esc_glcd_PARM_2
      000241 A2 05            [12] 2123 	mov	c,_ini_glcd_sloc0_1_0
      000243 92 04            [24] 2124 	mov	_esc_glcd_PARM_3,c
      000245 75 82 40         [24] 2125 	mov	dpl,#0x40
      000248 12 01 AB         [24] 2126 	lcall	_esc_glcd
                           0001A0  2127 	C$glcd.c$197$2$32 ==.
                                   2128 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:197: esc_glcd(0xb8, CO, cs); // X
      00024B C2 03            [12] 2129 	clr	_esc_glcd_PARM_2
      00024D A2 05            [12] 2130 	mov	c,_ini_glcd_sloc0_1_0
      00024F 92 04            [24] 2131 	mov	_esc_glcd_PARM_3,c
      000251 75 82 B8         [24] 2132 	mov	dpl,#0xb8
      000254 12 01 AB         [24] 2133 	lcall	_esc_glcd
                           0001AC  2134 	C$glcd.c$198$2$32 ==.
                                   2135 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:198: esc_glcd(0xc0, CO, cs); // Z
      000257 C2 03            [12] 2136 	clr	_esc_glcd_PARM_2
      000259 A2 05            [12] 2137 	mov	c,_ini_glcd_sloc0_1_0
      00025B 92 04            [24] 2138 	mov	_esc_glcd_PARM_3,c
      00025D 75 82 C0         [24] 2139 	mov	dpl,#0xc0
      000260 12 01 AB         [24] 2140 	lcall	_esc_glcd
      000263 D0 07            [24] 2141 	pop	ar7
                           0001BA  2142 	C$glcd.c$199$2$32 ==.
                                   2143 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:199: cs++;
      000265 0F               [12] 2144 	inc	r7
      000266 80 AD            [24] 2145 	sjmp	00104$
      000268                       2146 00107$:
                           0001BD  2147 	C$glcd.c$201$1$31 ==.
                           0001BD  2148 	XG$ini_glcd$0$0 ==.
      000268 22               [24] 2149 	ret
                                   2150 ;------------------------------------------------------------
                                   2151 ;Allocation info for local variables in function 'conf_Y'
                                   2152 ;------------------------------------------------------------
                                   2153 ;y                         Allocated to registers r7 
                                   2154 ;------------------------------------------------------------
                           0001BE  2155 	G$conf_Y$0$0 ==.
                           0001BE  2156 	C$glcd.c$203$1$31 ==.
                                   2157 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:203: void conf_Y(unsigned char y, __bit cs){
                                   2158 ;	-----------------------------------------
                                   2159 ;	 function conf_Y
                                   2160 ;	-----------------------------------------
      000269                       2161 _conf_Y:
      000269 AF 82            [24] 2162 	mov	r7,dpl
                           0001C0  2163 	C$glcd.c$206$1$34 ==.
                                   2164 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:206: y &= 0x3f; // para limitar o valor de Y de 0 ate 63
      00026B 53 07 3F         [24] 2165 	anl	ar7,#0x3f
                           0001C3  2166 	C$glcd.c$207$1$34 ==.
                                   2167 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:207: esc_glcd(0x40 | y, CO, cs);
      00026E 74 40            [12] 2168 	mov	a,#0x40
      000270 4F               [12] 2169 	orl	a,r7
      000271 F5 82            [12] 2170 	mov	dpl,a
      000273 C2 03            [12] 2171 	clr	_esc_glcd_PARM_2
      000275 A2 06            [12] 2172 	mov	c,_conf_Y_PARM_2
      000277 92 04            [24] 2173 	mov	_esc_glcd_PARM_3,c
      000279 12 01 AB         [24] 2174 	lcall	_esc_glcd
                           0001D1  2175 	C$glcd.c$208$1$34 ==.
                           0001D1  2176 	XG$conf_Y$0$0 ==.
      00027C 22               [24] 2177 	ret
                                   2178 ;------------------------------------------------------------
                                   2179 ;Allocation info for local variables in function 'conf_pag'
                                   2180 ;------------------------------------------------------------
                                   2181 ;pag                       Allocated to registers r7 
                                   2182 ;------------------------------------------------------------
                           0001D2  2183 	G$conf_pag$0$0 ==.
                           0001D2  2184 	C$glcd.c$211$1$34 ==.
                                   2185 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:211: void conf_pag(unsigned char pag, __bit cs){
                                   2186 ;	-----------------------------------------
                                   2187 ;	 function conf_pag
                                   2188 ;	-----------------------------------------
      00027D                       2189 _conf_pag:
      00027D AF 82            [24] 2190 	mov	r7,dpl
                           0001D4  2191 	C$glcd.c$214$1$36 ==.
                                   2192 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:214: pag &= 0x07; // Para limitar o valor de X de 0 ate 7
      00027F 53 07 07         [24] 2193 	anl	ar7,#0x07
                           0001D7  2194 	C$glcd.c$215$1$36 ==.
                                   2195 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:215: esc_glcd(0xb8 | pag, CO, cs);
      000282 74 B8            [12] 2196 	mov	a,#0xb8
      000284 4F               [12] 2197 	orl	a,r7
      000285 F5 82            [12] 2198 	mov	dpl,a
      000287 C2 03            [12] 2199 	clr	_esc_glcd_PARM_2
      000289 A2 07            [12] 2200 	mov	c,_conf_pag_PARM_2
      00028B 92 04            [24] 2201 	mov	_esc_glcd_PARM_3,c
      00028D 12 01 AB         [24] 2202 	lcall	_esc_glcd
                           0001E5  2203 	C$glcd.c$216$1$36 ==.
                           0001E5  2204 	XG$conf_pag$0$0 ==.
      000290 22               [24] 2205 	ret
                                   2206 ;------------------------------------------------------------
                                   2207 ;Allocation info for local variables in function 'limpa_glcd'
                                   2208 ;------------------------------------------------------------
                                   2209 ;x                         Allocated to registers r7 
                                   2210 ;y                         Allocated to registers r6 
                                   2211 ;------------------------------------------------------------
                           0001E6  2212 	G$limpa_glcd$0$0 ==.
                           0001E6  2213 	C$glcd.c$218$1$36 ==.
                                   2214 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:218: void limpa_glcd(__bit cs){
                                   2215 ;	-----------------------------------------
                                   2216 ;	 function limpa_glcd
                                   2217 ;	-----------------------------------------
      000291                       2218 _limpa_glcd:
                           0001E6  2219 	C$glcd.c$223$1$38 ==.
                                   2220 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:223: for(x=0; x<8; x++){
      000291 7F 00            [12] 2221 	mov	r7,#0x00
      000293                       2222 00105$:
                           0001E8  2223 	C$glcd.c$224$2$39 ==.
                                   2224 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:224: conf_pag(x, cs);
      000293 A2 08            [12] 2225 	mov	c,_limpa_glcd_PARM_1
      000295 92 07            [24] 2226 	mov	_conf_pag_PARM_2,c
      000297 8F 82            [24] 2227 	mov	dpl,r7
      000299 C0 07            [24] 2228 	push	ar7
      00029B 12 02 7D         [24] 2229 	lcall	_conf_pag
                           0001F3  2230 	C$glcd.c$225$2$39 ==.
                                   2231 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:225: conf_Y(0, cs);
      00029E A2 08            [12] 2232 	mov	c,_limpa_glcd_PARM_1
      0002A0 92 06            [24] 2233 	mov	_conf_Y_PARM_2,c
      0002A2 75 82 00         [24] 2234 	mov	dpl,#0x00
      0002A5 12 02 69         [24] 2235 	lcall	_conf_Y
      0002A8 D0 07            [24] 2236 	pop	ar7
                           0001FF  2237 	C$glcd.c$226$1$38 ==.
                                   2238 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:226: for(y=0; y<64; y++){
      0002AA 7E 00            [12] 2239 	mov	r6,#0x00
      0002AC                       2240 00103$:
                           000201  2241 	C$glcd.c$227$3$40 ==.
                                   2242 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:227: esc_glcd(0x00, DA, cs);
      0002AC D2 03            [12] 2243 	setb	_esc_glcd_PARM_2
      0002AE A2 08            [12] 2244 	mov	c,_limpa_glcd_PARM_1
      0002B0 92 04            [24] 2245 	mov	_esc_glcd_PARM_3,c
      0002B2 75 82 00         [24] 2246 	mov	dpl,#0x00
      0002B5 C0 07            [24] 2247 	push	ar7
      0002B7 C0 06            [24] 2248 	push	ar6
      0002B9 12 01 AB         [24] 2249 	lcall	_esc_glcd
      0002BC D0 06            [24] 2250 	pop	ar6
      0002BE D0 07            [24] 2251 	pop	ar7
                           000215  2252 	C$glcd.c$226$2$39 ==.
                                   2253 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:226: for(y=0; y<64; y++){
      0002C0 0E               [12] 2254 	inc	r6
      0002C1 BE 40 00         [24] 2255 	cjne	r6,#0x40,00120$
      0002C4                       2256 00120$:
      0002C4 40 E6            [24] 2257 	jc	00103$
                           00021B  2258 	C$glcd.c$223$1$38 ==.
                                   2259 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:223: for(x=0; x<8; x++){
      0002C6 0F               [12] 2260 	inc	r7
      0002C7 BF 08 00         [24] 2261 	cjne	r7,#0x08,00122$
      0002CA                       2262 00122$:
      0002CA 40 C7            [24] 2263 	jc	00105$
                           000221  2264 	C$glcd.c$230$1$38 ==.
                           000221  2265 	XG$limpa_glcd$0$0 ==.
      0002CC 22               [24] 2266 	ret
                                   2267 ;------------------------------------------------------------
                                   2268 ;Allocation info for local variables in function 'caractere_para_ascii'
                                   2269 ;------------------------------------------------------------
                                   2270 ;cod_ascii                 Allocated to registers r7 
                                   2271 ;------------------------------------------------------------
                           000222  2272 	G$caractere_para_ascii$0$0 ==.
                           000222  2273 	C$glcd.c$232$1$38 ==.
                                   2274 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:232: unsigned char caractere_para_ascii(unsigned char cod_ascii){
                                   2275 ;	-----------------------------------------
                                   2276 ;	 function caractere_para_ascii
                                   2277 ;	-----------------------------------------
      0002CD                       2278 _caractere_para_ascii:
      0002CD AF 82            [24] 2279 	mov	r7,dpl
                           000224  2280 	C$glcd.c$235$1$42 ==.
                                   2281 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:235: if(cod_ascii >= 32 && cod_ascii <= 127){
      0002CF BF 20 00         [24] 2282 	cjne	r7,#0x20,00118$
      0002D2                       2283 00118$:
      0002D2 40 0C            [24] 2284 	jc	00104$
      0002D4 EF               [12] 2285 	mov	a,r7
      0002D5 24 80            [12] 2286 	add	a,#0xff - 0x7f
      0002D7 40 07            [24] 2287 	jc	00104$
                           00022E  2288 	C$glcd.c$236$2$43 ==.
                                   2289 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:236: return cod_ascii - 32;
      0002D9 EF               [12] 2290 	mov	a,r7
      0002DA 24 E0            [12] 2291 	add	a,#0xe0
      0002DC F5 82            [12] 2292 	mov	dpl,a
      0002DE 80 0B            [24] 2293 	sjmp	00107$
      0002E0                       2294 00104$:
                           000235  2295 	C$glcd.c$237$1$42 ==.
                                   2296 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:237: }else if(cod_ascii == 176){
      0002E0 BF B0 05         [24] 2297 	cjne	r7,#0xb0,00105$
                           000238  2298 	C$glcd.c$238$2$44 ==.
                                   2299 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:238: return 96;
      0002E3 75 82 60         [24] 2300 	mov	dpl,#0x60
      0002E6 80 03            [24] 2301 	sjmp	00107$
      0002E8                       2302 00105$:
                           00023D  2303 	C$glcd.c$240$1$42 ==.
                                   2304 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:240: return 0;
      0002E8 75 82 00         [24] 2305 	mov	dpl,#0x00
      0002EB                       2306 00107$:
                           000240  2307 	C$glcd.c$241$1$42 ==.
                           000240  2308 	XG$caractere_para_ascii$0$0 ==.
      0002EB 22               [24] 2309 	ret
                                   2310 ;------------------------------------------------------------
                                   2311 ;Allocation info for local variables in function 'escreve_caractere'
                                   2312 ;------------------------------------------------------------
                                   2313 ;c                         Allocated to registers r7 
                                   2314 ;linha                     Allocated to registers r7 
                                   2315 ;------------------------------------------------------------
                           000241  2316 	G$escreve_caractere$0$0 ==.
                           000241  2317 	C$glcd.c$243$1$42 ==.
                                   2318 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:243: void escreve_caractere(char c, __bit cs){
                                   2319 ;	-----------------------------------------
                                   2320 ;	 function escreve_caractere
                                   2321 ;	-----------------------------------------
      0002EC                       2322 _escreve_caractere:
                           000241  2323 	C$glcd.c$246$1$46 ==.
                                   2324 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:246: unsigned char linha = caractere_para_ascii(c);
      0002EC 12 02 CD         [24] 2325 	lcall	_caractere_para_ascii
                           000244  2326 	C$glcd.c$248$1$46 ==.
                                   2327 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:248: esc_glcd(fonte[linha][0], DA, cs);
      0002EF E5 82            [12] 2328 	mov	a,dpl
      0002F1 75 F0 05         [24] 2329 	mov	b,#0x05
      0002F4 A4               [48] 2330 	mul	ab
      0002F5 24 A1            [12] 2331 	add	a,#_fonte
      0002F7 FE               [12] 2332 	mov	r6,a
      0002F8 74 15            [12] 2333 	mov	a,#(_fonte >> 8)
      0002FA 35 F0            [12] 2334 	addc	a,b
      0002FC FF               [12] 2335 	mov	r7,a
      0002FD 8E 82            [24] 2336 	mov	dpl,r6
      0002FF 8F 83            [24] 2337 	mov	dph,r7
      000301 E4               [12] 2338 	clr	a
      000302 93               [24] 2339 	movc	a,@a+dptr
      000303 FD               [12] 2340 	mov	r5,a
      000304 D2 03            [12] 2341 	setb	_esc_glcd_PARM_2
      000306 A2 09            [12] 2342 	mov	c,_escreve_caractere_PARM_2
      000308 92 04            [24] 2343 	mov	_esc_glcd_PARM_3,c
      00030A 8D 82            [24] 2344 	mov	dpl,r5
      00030C C0 07            [24] 2345 	push	ar7
      00030E C0 06            [24] 2346 	push	ar6
      000310 12 01 AB         [24] 2347 	lcall	_esc_glcd
      000313 D0 06            [24] 2348 	pop	ar6
      000315 D0 07            [24] 2349 	pop	ar7
                           00026C  2350 	C$glcd.c$249$1$46 ==.
                                   2351 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:249: esc_glcd(fonte[linha][1], DA, cs);
      000317 8E 82            [24] 2352 	mov	dpl,r6
      000319 8F 83            [24] 2353 	mov	dph,r7
      00031B A3               [24] 2354 	inc	dptr
      00031C E4               [12] 2355 	clr	a
      00031D 93               [24] 2356 	movc	a,@a+dptr
      00031E FD               [12] 2357 	mov	r5,a
      00031F D2 03            [12] 2358 	setb	_esc_glcd_PARM_2
      000321 A2 09            [12] 2359 	mov	c,_escreve_caractere_PARM_2
      000323 92 04            [24] 2360 	mov	_esc_glcd_PARM_3,c
      000325 8D 82            [24] 2361 	mov	dpl,r5
      000327 C0 07            [24] 2362 	push	ar7
      000329 C0 06            [24] 2363 	push	ar6
      00032B 12 01 AB         [24] 2364 	lcall	_esc_glcd
      00032E D0 06            [24] 2365 	pop	ar6
      000330 D0 07            [24] 2366 	pop	ar7
                           000287  2367 	C$glcd.c$250$1$46 ==.
                                   2368 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:250: esc_glcd(fonte[linha][2], DA, cs);
      000332 8E 82            [24] 2369 	mov	dpl,r6
      000334 8F 83            [24] 2370 	mov	dph,r7
      000336 A3               [24] 2371 	inc	dptr
      000337 A3               [24] 2372 	inc	dptr
      000338 E4               [12] 2373 	clr	a
      000339 93               [24] 2374 	movc	a,@a+dptr
      00033A FD               [12] 2375 	mov	r5,a
      00033B D2 03            [12] 2376 	setb	_esc_glcd_PARM_2
      00033D A2 09            [12] 2377 	mov	c,_escreve_caractere_PARM_2
      00033F 92 04            [24] 2378 	mov	_esc_glcd_PARM_3,c
      000341 8D 82            [24] 2379 	mov	dpl,r5
      000343 C0 07            [24] 2380 	push	ar7
      000345 C0 06            [24] 2381 	push	ar6
      000347 12 01 AB         [24] 2382 	lcall	_esc_glcd
      00034A D0 06            [24] 2383 	pop	ar6
      00034C D0 07            [24] 2384 	pop	ar7
                           0002A3  2385 	C$glcd.c$251$1$46 ==.
                                   2386 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:251: esc_glcd(fonte[linha][3], DA, cs);
      00034E 8E 82            [24] 2387 	mov	dpl,r6
      000350 8F 83            [24] 2388 	mov	dph,r7
      000352 A3               [24] 2389 	inc	dptr
      000353 A3               [24] 2390 	inc	dptr
      000354 A3               [24] 2391 	inc	dptr
      000355 E4               [12] 2392 	clr	a
      000356 93               [24] 2393 	movc	a,@a+dptr
      000357 FD               [12] 2394 	mov	r5,a
      000358 D2 03            [12] 2395 	setb	_esc_glcd_PARM_2
      00035A A2 09            [12] 2396 	mov	c,_escreve_caractere_PARM_2
      00035C 92 04            [24] 2397 	mov	_esc_glcd_PARM_3,c
      00035E 8D 82            [24] 2398 	mov	dpl,r5
      000360 C0 07            [24] 2399 	push	ar7
      000362 C0 06            [24] 2400 	push	ar6
      000364 12 01 AB         [24] 2401 	lcall	_esc_glcd
      000367 D0 06            [24] 2402 	pop	ar6
      000369 D0 07            [24] 2403 	pop	ar7
                           0002C0  2404 	C$glcd.c$252$1$46 ==.
                                   2405 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:252: esc_glcd(fonte[linha][4], DA, cs);
      00036B 8E 82            [24] 2406 	mov	dpl,r6
      00036D 8F 83            [24] 2407 	mov	dph,r7
      00036F A3               [24] 2408 	inc	dptr
      000370 A3               [24] 2409 	inc	dptr
      000371 A3               [24] 2410 	inc	dptr
      000372 A3               [24] 2411 	inc	dptr
      000373 E4               [12] 2412 	clr	a
      000374 93               [24] 2413 	movc	a,@a+dptr
      000375 FF               [12] 2414 	mov	r7,a
      000376 D2 03            [12] 2415 	setb	_esc_glcd_PARM_2
      000378 A2 09            [12] 2416 	mov	c,_escreve_caractere_PARM_2
      00037A 92 04            [24] 2417 	mov	_esc_glcd_PARM_3,c
      00037C 8F 82            [24] 2418 	mov	dpl,r7
      00037E 12 01 AB         [24] 2419 	lcall	_esc_glcd
                           0002D6  2420 	C$glcd.c$253$1$46 ==.
                                   2421 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:253: esc_glcd(0x00, DA, cs);
      000381 D2 03            [12] 2422 	setb	_esc_glcd_PARM_2
      000383 A2 09            [12] 2423 	mov	c,_escreve_caractere_PARM_2
      000385 92 04            [24] 2424 	mov	_esc_glcd_PARM_3,c
      000387 75 82 00         [24] 2425 	mov	dpl,#0x00
      00038A 12 01 AB         [24] 2426 	lcall	_esc_glcd
                           0002E2  2427 	C$glcd.c$254$1$46 ==.
                                   2428 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:254: esc_glcd(0x00, DA, cs);
      00038D D2 03            [12] 2429 	setb	_esc_glcd_PARM_2
      00038F A2 09            [12] 2430 	mov	c,_escreve_caractere_PARM_2
      000391 92 04            [24] 2431 	mov	_esc_glcd_PARM_3,c
      000393 75 82 00         [24] 2432 	mov	dpl,#0x00
      000396 12 01 AB         [24] 2433 	lcall	_esc_glcd
                           0002EE  2434 	C$glcd.c$255$1$46 ==.
                                   2435 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:255: esc_glcd(0x00, DA, cs);
      000399 D2 03            [12] 2436 	setb	_esc_glcd_PARM_2
      00039B A2 09            [12] 2437 	mov	c,_escreve_caractere_PARM_2
      00039D 92 04            [24] 2438 	mov	_esc_glcd_PARM_3,c
      00039F 75 82 00         [24] 2439 	mov	dpl,#0x00
      0003A2 12 01 AB         [24] 2440 	lcall	_esc_glcd
                           0002FA  2441 	C$glcd.c$256$1$46 ==.
                           0002FA  2442 	XG$escreve_caractere$0$0 ==.
      0003A5 22               [24] 2443 	ret
                                   2444 ;------------------------------------------------------------
                                   2445 ;Allocation info for local variables in function 'putchar'
                                   2446 ;------------------------------------------------------------
                                   2447 ;c                         Allocated to registers r7 
                                   2448 ;------------------------------------------------------------
                           0002FB  2449 	G$putchar$0$0 ==.
                           0002FB  2450 	C$glcd.c$258$1$46 ==.
                                   2451 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:258: void putchar(char c){
                                   2452 ;	-----------------------------------------
                                   2453 ;	 function putchar
                                   2454 ;	-----------------------------------------
      0003A6                       2455 _putchar:
      0003A6 AF 82            [24] 2456 	mov	r7,dpl
                           0002FD  2457 	C$glcd.c$265$1$48 ==.
                                   2458 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:265: WDTCN = 0xa5;
      0003A8 75 FF A5         [24] 2459 	mov	_WDTCN,#0xa5
                           000300  2460 	C$glcd.c$267$1$48 ==.
                                   2461 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:267: if(c<=8){
      0003AB EF               [12] 2462 	mov	a,r7
      0003AC 24 F7            [12] 2463 	add	a,#0xff - 0x08
      0003AE 40 2C            [24] 2464 	jc	00112$
                           000305  2465 	C$glcd.c$268$2$49 ==.
                                   2466 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:268: conf_pag(c-1, ESQ);
      0003B0 EF               [12] 2467 	mov	a,r7
      0003B1 14               [12] 2468 	dec	a
      0003B2 FE               [12] 2469 	mov	r6,a
      0003B3 C2 07            [12] 2470 	clr	_conf_pag_PARM_2
      0003B5 8E 82            [24] 2471 	mov	dpl,r6
      0003B7 C0 06            [24] 2472 	push	ar6
      0003B9 12 02 7D         [24] 2473 	lcall	_conf_pag
                           000311  2474 	C$glcd.c$269$2$49 ==.
                                   2475 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:269: conf_Y(0, ESQ);
      0003BC C2 06            [12] 2476 	clr	_conf_Y_PARM_2
      0003BE 75 82 00         [24] 2477 	mov	dpl,#0x00
      0003C1 12 02 69         [24] 2478 	lcall	_conf_Y
      0003C4 D0 06            [24] 2479 	pop	ar6
                           00031B  2480 	C$glcd.c$270$2$49 ==.
                                   2481 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:270: conf_pag(c-1, DIR);
      0003C6 D2 07            [12] 2482 	setb	_conf_pag_PARM_2
      0003C8 8E 82            [24] 2483 	mov	dpl,r6
      0003CA 12 02 7D         [24] 2484 	lcall	_conf_pag
                           000322  2485 	C$glcd.c$271$2$49 ==.
                                   2486 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:271: conf_Y(0, DIR);
      0003CD D2 06            [12] 2487 	setb	_conf_Y_PARM_2
      0003CF 75 82 00         [24] 2488 	mov	dpl,#0x00
      0003D2 12 02 69         [24] 2489 	lcall	_conf_Y
                           00032A  2490 	C$glcd.c$272$2$49 ==.
                                   2491 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:272: conta_caractere = 0;
      0003D5 75 24 00         [24] 2492 	mov	_conta_caractere,#0x00
                           00032D  2493 	C$glcd.c$273$2$49 ==.
                                   2494 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:273: terminal_ativo = 0;
      0003D8 C2 00            [12] 2495 	clr	_terminal_ativo
      0003DA 80 22            [24] 2496 	sjmp	00114$
      0003DC                       2497 00112$:
                           000331  2498 	C$glcd.c$275$1$48 ==.
                                   2499 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:275: }else if(c == 9 || terminal_ativo == 1){
      0003DC BF 09 02         [24] 2500 	cjne	r7,#0x09,00132$
      0003DF 80 03            [24] 2501 	sjmp	00107$
      0003E1                       2502 00132$:
      0003E1 30 00 09         [24] 2503 	jnb	_terminal_ativo,00108$
      0003E4                       2504 00107$:
                           000339  2505 	C$glcd.c$276$2$50 ==.
                                   2506 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:276: terminal_ativo = 1;
      0003E4 D2 00            [12] 2507 	setb	_terminal_ativo
                           00033B  2508 	C$glcd.c$277$2$50 ==.
                                   2509 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:277: SBUF0 = c;
      0003E6 8F 99            [24] 2510 	mov	_SBUF0,r7
                           00033D  2511 	C$glcd.c$278$2$50 ==.
                                   2512 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:278: while(TI0==0);
      0003E8                       2513 00101$:
                           00033D  2514 	C$glcd.c$279$2$50 ==.
                                   2515 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:279: TI0 = 0;
      0003E8 10 99 13         [24] 2516 	jbc	_TI0,00114$
      0003EB 80 FB            [24] 2517 	sjmp	00101$
      0003ED                       2518 00108$:
                           000342  2519 	C$glcd.c$282$2$51 ==.
                                   2520 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:282: if(conta_caractere<8){
      0003ED 74 F8            [12] 2521 	mov	a,#0x100 - 0x08
      0003EF 25 24            [12] 2522 	add	a,_conta_caractere
                           000346  2523 	C$glcd.c$283$3$52 ==.
                                   2524 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:283: lado = ESQ;
                           000346  2525 	C$glcd.c$285$3$53 ==.
                                   2526 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:285: lado = DIR;
      0003F1 92 0A            [24] 2527 	mov	_putchar_lado_1_48,c
                           000348  2528 	C$glcd.c$288$2$51 ==.
                                   2529 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:288: escreve_caractere(c, lado);
      0003F3 A2 0A            [12] 2530 	mov	c,_putchar_lado_1_48
      0003F5 92 09            [24] 2531 	mov	_escreve_caractere_PARM_2,c
      0003F7 8F 82            [24] 2532 	mov	dpl,r7
      0003F9 12 02 EC         [24] 2533 	lcall	_escreve_caractere
                           000351  2534 	C$glcd.c$289$2$51 ==.
                                   2535 ;	C:\Users\202019050584\Desktop\Trabalho\/glcd.c:289: conta_caractere++;
      0003FC 05 24            [12] 2536 	inc	_conta_caractere
      0003FE                       2537 00114$:
                           000353  2538 	C$glcd.c$291$1$48 ==.
                           000353  2539 	XG$putchar$0$0 ==.
      0003FE 22               [24] 2540 	ret
                                   2541 ;------------------------------------------------------------
                                   2542 ;Allocation info for local variables in function 'delay_ms'
                                   2543 ;------------------------------------------------------------
                                   2544 ;t                         Allocated to registers r6 r7 
                                   2545 ;------------------------------------------------------------
                           000354  2546 	G$delay_ms$0$0 ==.
                           000354  2547 	C$delay.c$1$1$48 ==.
                                   2548 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:1: void delay_ms(unsigned int t){
                                   2549 ;	-----------------------------------------
                                   2550 ;	 function delay_ms
                                   2551 ;	-----------------------------------------
      0003FF                       2552 _delay_ms:
      0003FF AE 82            [24] 2553 	mov	r6,dpl
      000401 AF 83            [24] 2554 	mov	r7,dph
                           000358  2555 	C$delay.c$2$1$55 ==.
                                   2556 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:2: TMOD |= 0x01;
      000403 43 89 01         [24] 2557 	orl	_TMOD,#0x01
                           00035B  2558 	C$delay.c$3$1$55 ==.
                                   2559 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:3: TMOD &= ~0x02;
      000406 53 89 FD         [24] 2560 	anl	_TMOD,#0xfd
      000409                       2561 00106$:
                           00035E  2562 	C$delay.c$4$1$55 ==.
                                   2563 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:4: for(;t>0;t--){
      000409 EE               [12] 2564 	mov	a,r6
      00040A 4F               [12] 2565 	orl	a,r7
      00040B 60 19            [24] 2566 	jz	00108$
                           000362  2567 	C$delay.c$5$2$56 ==.
                                   2568 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:5: WDTCN = 0xa5;
      00040D 75 FF A5         [24] 2569 	mov	_WDTCN,#0xa5
                           000365  2570 	C$delay.c$6$2$56 ==.
                                   2571 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:6: TR0 = 0;
      000410 C2 8C            [12] 2572 	clr	_TR0
                           000367  2573 	C$delay.c$7$2$56 ==.
                                   2574 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:7: TF0 = 0;
      000412 C2 8D            [12] 2575 	clr	_TF0
                           000369  2576 	C$delay.c$8$2$56 ==.
                                   2577 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:8: TL0 = 0x58;
      000414 75 8A 58         [24] 2578 	mov	_TL0,#0x58
                           00036C  2579 	C$delay.c$9$2$56 ==.
                                   2580 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:9: TH0 = 0x9E;
      000417 75 8C 9E         [24] 2581 	mov	_TH0,#0x9e
                           00036F  2582 	C$delay.c$10$2$56 ==.
                                   2583 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:10: TR0 = 1;
      00041A D2 8C            [12] 2584 	setb	_TR0
                           000371  2585 	C$delay.c$11$2$56 ==.
                                   2586 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:11: while(TF0 == 0);
      00041C                       2587 00101$:
      00041C 30 8D FD         [24] 2588 	jnb	_TF0,00101$
                           000374  2589 	C$delay.c$4$1$55 ==.
                                   2590 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:4: for(;t>0;t--){
      00041F 1E               [12] 2591 	dec	r6
      000420 BE FF 01         [24] 2592 	cjne	r6,#0xff,00127$
      000423 1F               [12] 2593 	dec	r7
      000424                       2594 00127$:
      000424 80 E3            [24] 2595 	sjmp	00106$
      000426                       2596 00108$:
                           00037B  2597 	C$delay.c$13$1$55 ==.
                           00037B  2598 	XG$delay_ms$0$0 ==.
      000426 22               [24] 2599 	ret
                                   2600 ;------------------------------------------------------------
                                   2601 ;Allocation info for local variables in function 'delay_us'
                                   2602 ;------------------------------------------------------------
                                   2603 ;t                         Allocated to registers r6 r7 
                                   2604 ;------------------------------------------------------------
                           00037C  2605 	G$delay_us$0$0 ==.
                           00037C  2606 	C$delay.c$15$1$55 ==.
                                   2607 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:15: void delay_us(unsigned int t){
                                   2608 ;	-----------------------------------------
                                   2609 ;	 function delay_us
                                   2610 ;	-----------------------------------------
      000427                       2611 _delay_us:
      000427 AE 82            [24] 2612 	mov	r6,dpl
      000429 AF 83            [24] 2613 	mov	r7,dph
                           000380  2614 	C$delay.c$16$1$58 ==.
                                   2615 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:16: TMOD |= 0X02;
      00042B 43 89 02         [24] 2616 	orl	_TMOD,#0x02
                           000383  2617 	C$delay.c$17$1$58 ==.
                                   2618 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:17: TMOD &= ~0X01;
      00042E 53 89 FE         [24] 2619 	anl	_TMOD,#0xfe
                           000386  2620 	C$delay.c$18$1$58 ==.
                                   2621 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:18: TR0 = 0;
      000431 C2 8C            [12] 2622 	clr	_TR0
                           000388  2623 	C$delay.c$19$1$58 ==.
                                   2624 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:19: TF0 = 0;
      000433 C2 8D            [12] 2625 	clr	_TF0
                           00038A  2626 	C$delay.c$20$1$58 ==.
                                   2627 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:20: TL0 = 0xE7;
      000435 75 8A E7         [24] 2628 	mov	_TL0,#0xe7
                           00038D  2629 	C$delay.c$21$1$58 ==.
                                   2630 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:21: TH0 = 0xE7;
      000438 75 8C E7         [24] 2631 	mov	_TH0,#0xe7
                           000390  2632 	C$delay.c$22$1$58 ==.
                                   2633 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:22: TR0 = 1;
      00043B D2 8C            [12] 2634 	setb	_TR0
      00043D                       2635 00106$:
                           000392  2636 	C$delay.c$23$1$58 ==.
                                   2637 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:23: for(;t>0;t--){
      00043D EE               [12] 2638 	mov	a,r6
      00043E 4F               [12] 2639 	orl	a,r7
      00043F 60 0F            [24] 2640 	jz	00108$
                           000396  2641 	C$delay.c$24$2$59 ==.
                                   2642 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:24: WDTCN = 0xa5;
      000441 75 FF A5         [24] 2643 	mov	_WDTCN,#0xa5
                           000399  2644 	C$delay.c$25$2$59 ==.
                                   2645 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:25: while(TF0 == 0);
      000444                       2646 00101$:
                           000399  2647 	C$delay.c$26$2$59 ==.
                                   2648 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:26: TF0 = 0;
      000444 10 8D 02         [24] 2649 	jbc	_TF0,00126$
      000447 80 FB            [24] 2650 	sjmp	00101$
      000449                       2651 00126$:
                           00039E  2652 	C$delay.c$23$1$58 ==.
                                   2653 ;	C:\Users\202019050584\Desktop\Trabalho\/delay.c:23: for(;t>0;t--){
      000449 1E               [12] 2654 	dec	r6
      00044A BE FF 01         [24] 2655 	cjne	r6,#0xff,00127$
      00044D 1F               [12] 2656 	dec	r7
      00044E                       2657 00127$:
      00044E 80 ED            [24] 2658 	sjmp	00106$
      000450                       2659 00108$:
                           0003A5  2660 	C$delay.c$29$1$58 ==.
                           0003A5  2661 	XG$delay_us$0$0 ==.
      000450 22               [24] 2662 	ret
                                   2663 ;------------------------------------------------------------
                                   2664 ;Allocation info for local variables in function 'inicia_dht11'
                                   2665 ;------------------------------------------------------------
                           0003A6  2666 	G$inicia_dht11$0$0 ==.
                           0003A6  2667 	C$sensores.c$48$1$58 ==.
                                   2668 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:48: void inicia_dht11(void){
                                   2669 ;	-----------------------------------------
                                   2670 ;	 function inicia_dht11
                                   2671 ;	-----------------------------------------
      000451                       2672 _inicia_dht11:
                           0003A6  2673 	C$sensores.c$51$1$61 ==.
                                   2674 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:51: DHT11=0;
      000451 C2 87            [12] 2675 	clr	_P0_7
                           0003A8  2676 	C$sensores.c$52$1$61 ==.
                                   2677 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:52: delay_ms(18);
      000453 90 00 12         [24] 2678 	mov	dptr,#0x0012
      000456 12 03 FF         [24] 2679 	lcall	_delay_ms
                           0003AE  2680 	C$sensores.c$53$1$61 ==.
                                   2681 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:53: DHT11=1;
      000459 D2 87            [12] 2682 	setb	_P0_7
                           0003B0  2683 	C$sensores.c$54$1$61 ==.
                                   2684 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:54: delay_us(30);
      00045B 90 00 1E         [24] 2685 	mov	dptr,#0x001e
      00045E 12 04 27         [24] 2686 	lcall	_delay_us
                           0003B6  2687 	C$sensores.c$55$1$61 ==.
                           0003B6  2688 	XG$inicia_dht11$0$0 ==.
      000461 22               [24] 2689 	ret
                                   2690 ;------------------------------------------------------------
                                   2691 ;Allocation info for local variables in function 'resposta_dht11'
                                   2692 ;------------------------------------------------------------
                           0003B7  2693 	G$resposta_dht11$0$0 ==.
                           0003B7  2694 	C$sensores.c$57$1$61 ==.
                                   2695 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:57: void resposta_dht11(void){
                                   2696 ;	-----------------------------------------
                                   2697 ;	 function resposta_dht11
                                   2698 ;	-----------------------------------------
      000462                       2699 _resposta_dht11:
                           0003B7  2700 	C$sensores.c$60$1$63 ==.
                                   2701 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:60: transmissao_dht11 = 0;
      000462 C2 0B            [12] 2702 	clr	_transmissao_dht11
                           0003B9  2703 	C$sensores.c$61$1$63 ==.
                                   2704 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:61: delay_us(40);
      000464 90 00 28         [24] 2705 	mov	dptr,#0x0028
      000467 12 04 27         [24] 2706 	lcall	_delay_us
                           0003BF  2707 	C$sensores.c$62$1$63 ==.
                                   2708 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:62: if(DHT11 == 0){
      00046A 20 87 11         [24] 2709 	jb	_P0_7,00105$
                           0003C2  2710 	C$sensores.c$63$2$64 ==.
                                   2711 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:63: delay_us(80);
      00046D 90 00 50         [24] 2712 	mov	dptr,#0x0050
      000470 12 04 27         [24] 2713 	lcall	_delay_us
                           0003C8  2714 	C$sensores.c$64$2$64 ==.
                                   2715 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:64: if(DHT11 == 1) transmissao_dht11 = 1;
      000473 30 87 02         [24] 2716 	jnb	_P0_7,00102$
      000476 D2 0B            [12] 2717 	setb	_transmissao_dht11
      000478                       2718 00102$:
                           0003CD  2719 	C$sensores.c$65$2$64 ==.
                                   2720 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:65: delay_us(50);
      000478 90 00 32         [24] 2721 	mov	dptr,#0x0032
      00047B 12 04 27         [24] 2722 	lcall	_delay_us
      00047E                       2723 00105$:
                           0003D3  2724 	C$sensores.c$69$1$63 ==.
                           0003D3  2725 	XG$resposta_dht11$0$0 ==.
      00047E 22               [24] 2726 	ret
                                   2727 ;------------------------------------------------------------
                                   2728 ;Allocation info for local variables in function 'le_byte_dht11'
                                   2729 ;------------------------------------------------------------
                                   2730 ;i                         Allocated to registers r6 
                                   2731 ;byte                      Allocated to registers r7 
                                   2732 ;------------------------------------------------------------
                           0003D4  2733 	G$le_byte_dht11$0$0 ==.
                           0003D4  2734 	C$sensores.c$71$1$63 ==.
                                   2735 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:71: unsigned char le_byte_dht11(void){
                                   2736 ;	-----------------------------------------
                                   2737 ;	 function le_byte_dht11
                                   2738 ;	-----------------------------------------
      00047F                       2739 _le_byte_dht11:
                           0003D4  2740 	C$sensores.c$74$1$63 ==.
                                   2741 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:74: unsigned char i, byte=0;
      00047F 7F 00            [12] 2742 	mov	r7,#0x00
                           0003D6  2743 	C$sensores.c$77$1$66 ==.
                                   2744 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:77: while(DHT11==0);
      000481 7E 00            [12] 2745 	mov	r6,#0x00
      000483                       2746 00101$:
      000483 30 87 FD         [24] 2747 	jnb	_P0_7,00101$
                           0003DB  2748 	C$sensores.c$78$2$67 ==.
                                   2749 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:78: delay_us(40);
      000486 90 00 28         [24] 2750 	mov	dptr,#0x0028
      000489 C0 07            [24] 2751 	push	ar7
      00048B C0 06            [24] 2752 	push	ar6
      00048D 12 04 27         [24] 2753 	lcall	_delay_us
      000490 D0 06            [24] 2754 	pop	ar6
      000492 D0 07            [24] 2755 	pop	ar7
                           0003E9  2756 	C$sensores.c$80$2$67 ==.
                                   2757 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:80: if(DHT11==1) byte = (byte<<1) | (0x01);
      000494 30 87 09         [24] 2758 	jnb	_P0_7,00105$
      000497 EF               [12] 2759 	mov	a,r7
      000498 2F               [12] 2760 	add	a,r7
      000499 FD               [12] 2761 	mov	r5,a
      00049A 74 01            [12] 2762 	mov	a,#0x01
      00049C 4D               [12] 2763 	orl	a,r5
      00049D FF               [12] 2764 	mov	r7,a
      00049E 80 03            [24] 2765 	sjmp	00107$
      0004A0                       2766 00105$:
                           0003F5  2767 	C$sensores.c$81$2$67 ==.
                                   2768 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:81: else byte = (byte<<1);
      0004A0 EF               [12] 2769 	mov	a,r7
      0004A1 2F               [12] 2770 	add	a,r7
      0004A2 FF               [12] 2771 	mov	r7,a
                           0003F8  2772 	C$sensores.c$83$2$67 ==.
                                   2773 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:83: while(DHT11==1);
      0004A3                       2774 00107$:
      0004A3 20 87 FD         [24] 2775 	jb	_P0_7,00107$
                           0003FB  2776 	C$sensores.c$76$1$66 ==.
                                   2777 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:76: for(i = 0; i < 8; i++){
      0004A6 0E               [12] 2778 	inc	r6
      0004A7 BE 08 00         [24] 2779 	cjne	r6,#0x08,00137$
      0004AA                       2780 00137$:
      0004AA 40 D7            [24] 2781 	jc	00101$
                           000401  2782 	C$sensores.c$86$1$66 ==.
                                   2783 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:86: return byte;
      0004AC 8F 82            [24] 2784 	mov	dpl,r7
                           000403  2785 	C$sensores.c$87$1$66 ==.
                           000403  2786 	XG$le_byte_dht11$0$0 ==.
      0004AE 22               [24] 2787 	ret
                                   2788 ;------------------------------------------------------------
                                   2789 ;Allocation info for local variables in function 'le_dht11'
                                   2790 ;------------------------------------------------------------
                                   2791 ;d_rh                      Allocated to registers r7 
                                   2792 ;d_temp                    Allocated to registers r6 
                                   2793 ;checksum                  Allocated to registers r5 
                                   2794 ;------------------------------------------------------------
                           000404  2795 	G$le_dht11$0$0 ==.
                           000404  2796 	C$sensores.c$89$1$66 ==.
                                   2797 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:89: void le_dht11(void){
                                   2798 ;	-----------------------------------------
                                   2799 ;	 function le_dht11
                                   2800 ;	-----------------------------------------
      0004AF                       2801 _le_dht11:
                           000404  2802 	C$sensores.c$94$1$69 ==.
                                   2803 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:94: inicia_dht11();
      0004AF 12 04 51         [24] 2804 	lcall	_inicia_dht11
                           000407  2805 	C$sensores.c$95$1$69 ==.
                                   2806 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:95: resposta_dht11();
      0004B2 12 04 62         [24] 2807 	lcall	_resposta_dht11
                           00040A  2808 	C$sensores.c$97$1$69 ==.
                                   2809 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:97: if(transmissao_dht11 == 1){
      0004B5 30 0B 5A         [24] 2810 	jnb	_transmissao_dht11,00105$
                           00040D  2811 	C$sensores.c$98$2$70 ==.
                                   2812 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:98: saida[I_RH] = le_byte_dht11();
      0004B8 12 04 7F         [24] 2813 	lcall	_le_byte_dht11
      0004BB E5 82            [12] 2814 	mov	a,dpl
      0004BD F5 26            [12] 2815 	mov	(_saida + 0x0001),a
                           000414  2816 	C$sensores.c$99$2$70 ==.
                                   2817 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:99: d_rh = le_byte_dht11();
      0004BF 12 04 7F         [24] 2818 	lcall	_le_byte_dht11
      0004C2 AF 82            [24] 2819 	mov	r7,dpl
                           000419  2820 	C$sensores.c$100$2$70 ==.
                                   2821 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:100: saida[I_TEMP] = le_byte_dht11();
      0004C4 C0 07            [24] 2822 	push	ar7
      0004C6 12 04 7F         [24] 2823 	lcall	_le_byte_dht11
      0004C9 E5 82            [12] 2824 	mov	a,dpl
      0004CB F5 27            [12] 2825 	mov	(_saida + 0x0002),a
                           000422  2826 	C$sensores.c$101$2$70 ==.
                                   2827 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:101: d_temp = le_byte_dht11();
      0004CD 12 04 7F         [24] 2828 	lcall	_le_byte_dht11
      0004D0 AE 82            [24] 2829 	mov	r6,dpl
                           000427  2830 	C$sensores.c$102$2$70 ==.
                                   2831 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:102: checksum = le_byte_dht11();
      0004D2 C0 06            [24] 2832 	push	ar6
      0004D4 12 04 7F         [24] 2833 	lcall	_le_byte_dht11
      0004D7 AD 82            [24] 2834 	mov	r5,dpl
      0004D9 D0 06            [24] 2835 	pop	ar6
      0004DB D0 07            [24] 2836 	pop	ar7
                           000432  2837 	C$sensores.c$104$2$70 ==.
                                   2838 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:104: if((saida[I_RH]+d_rh+saida[I_TEMP]+d_temp) == checksum){
      0004DD AB 26            [24] 2839 	mov	r3,(_saida + 0x0001)
      0004DF E4               [12] 2840 	clr	a
      0004E0 FC               [12] 2841 	mov	r4,a
      0004E1 FA               [12] 2842 	mov	r2,a
      0004E2 EF               [12] 2843 	mov	a,r7
      0004E3 2B               [12] 2844 	add	a,r3
      0004E4 FB               [12] 2845 	mov	r3,a
      0004E5 EA               [12] 2846 	mov	a,r2
      0004E6 3C               [12] 2847 	addc	a,r4
      0004E7 FC               [12] 2848 	mov	r4,a
      0004E8 AA 27            [24] 2849 	mov	r2,(_saida + 0x0002)
      0004EA 7F 00            [12] 2850 	mov	r7,#0x00
      0004EC EA               [12] 2851 	mov	a,r2
      0004ED 2B               [12] 2852 	add	a,r3
      0004EE FB               [12] 2853 	mov	r3,a
      0004EF EF               [12] 2854 	mov	a,r7
      0004F0 3C               [12] 2855 	addc	a,r4
      0004F1 FC               [12] 2856 	mov	r4,a
      0004F2 7F 00            [12] 2857 	mov	r7,#0x00
      0004F4 EE               [12] 2858 	mov	a,r6
      0004F5 2B               [12] 2859 	add	a,r3
      0004F6 FB               [12] 2860 	mov	r3,a
      0004F7 EF               [12] 2861 	mov	a,r7
      0004F8 3C               [12] 2862 	addc	a,r4
      0004F9 FC               [12] 2863 	mov	r4,a
      0004FA 7F 00            [12] 2864 	mov	r7,#0x00
      0004FC EB               [12] 2865 	mov	a,r3
      0004FD B5 05 0B         [24] 2866 	cjne	a,ar5,00102$
      000500 EC               [12] 2867 	mov	a,r4
      000501 B5 07 07         [24] 2868 	cjne	a,ar7,00102$
                           000459  2869 	C$sensores.c$105$3$71 ==.
                                   2870 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:105: saida[CHECK] = 1;
      000504 75 25 01         [24] 2871 	mov	_saida,#0x01
                           00045C  2872 	C$sensores.c$106$3$71 ==.
                                   2873 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:106: P3_0 = 0;
      000507 C2 B0            [12] 2874 	clr	_P3_0
      000509 80 0C            [24] 2875 	sjmp	00107$
      00050B                       2876 00102$:
                           000460  2877 	C$sensores.c$108$3$72 ==.
                                   2878 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:108: saida[CHECK] = 2;
      00050B 75 25 02         [24] 2879 	mov	_saida,#0x02
                           000463  2880 	C$sensores.c$109$3$72 ==.
                                   2881 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:109: P3_0 = 1;
      00050E D2 B0            [12] 2882 	setb	_P3_0
      000510 80 05            [24] 2883 	sjmp	00107$
      000512                       2884 00105$:
                           000467  2885 	C$sensores.c$112$2$73 ==.
                                   2886 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:112: saida[CHECK] = 0;
      000512 75 25 00         [24] 2887 	mov	_saida,#0x00
                           00046A  2888 	C$sensores.c$113$2$73 ==.
                                   2889 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:113: P3_0 = 1;
      000515 D2 B0            [12] 2890 	setb	_P3_0
      000517                       2891 00107$:
                           00046C  2892 	C$sensores.c$115$1$69 ==.
                           00046C  2893 	XG$le_dht11$0$0 ==.
      000517 22               [24] 2894 	ret
                                   2895 ;------------------------------------------------------------
                                   2896 ;Allocation info for local variables in function 'le_adc0'
                                   2897 ;------------------------------------------------------------
                                   2898 ;ganho                     Allocated with name '_le_adc0_PARM_2'
                                   2899 ;indice_high               Allocated with name '_le_adc0_PARM_3'
                                   2900 ;indice_low                Allocated with name '_le_adc0_PARM_4'
                                   2901 ;canal                     Allocated to registers r7 
                                   2902 ;------------------------------------------------------------
                           00046D  2903 	G$le_adc0$0$0 ==.
                           00046D  2904 	C$sensores.c$117$1$69 ==.
                                   2905 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:117: void le_adc0(unsigned char canal, unsigned char ganho, unsigned char indice_high, unsigned char indice_low){
                                   2906 ;	-----------------------------------------
                                   2907 ;	 function le_adc0
                                   2908 ;	-----------------------------------------
      000518                       2909 _le_adc0:
      000518 AF 82            [24] 2910 	mov	r7,dpl
                           00046F  2911 	C$sensores.c$120$1$75 ==.
                                   2912 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:120: ADC0CF = (ADC0CF & 0xf8) | ganho;
      00051A 74 F8            [12] 2913 	mov	a,#0xf8
      00051C 55 BC            [12] 2914 	anl	a,_ADC0CF
      00051E 45 0F            [12] 2915 	orl	a,_le_adc0_PARM_2
      000520 F5 BC            [12] 2916 	mov	_ADC0CF,a
                           000477  2917 	C$sensores.c$121$1$75 ==.
                                   2918 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:121: AMX0SL = canal;
      000522 8F BB            [24] 2919 	mov	_AMX0SL,r7
                           000479  2920 	C$sensores.c$123$1$75 ==.
                                   2921 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:123: AD0BUSY = 1; // Inicia a conversao
      000524 D2 EC            [12] 2922 	setb	_AD0BUSY
                           00047B  2923 	C$sensores.c$124$1$75 ==.
                                   2924 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:124: NOP();
      000526 00               [12] 2925 	NOP	
                           00047C  2926 	C$sensores.c$125$1$75 ==.
                                   2927 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:125: while(AD0BUSY); // Aguarda a conversao
      000527                       2928 00101$:
      000527 20 EC FD         [24] 2929 	jb	_AD0BUSY,00101$
                           00047F  2930 	C$sensores.c$127$1$75 ==.
                                   2931 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:127: saida[indice_high] = ADC0H;
      00052A E5 10            [12] 2932 	mov	a,_le_adc0_PARM_3
      00052C 24 25            [12] 2933 	add	a,#_saida
      00052E F8               [12] 2934 	mov	r0,a
      00052F A6 BF            [24] 2935 	mov	@r0,_ADC0H
                           000486  2936 	C$sensores.c$128$1$75 ==.
                                   2937 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:128: saida[indice_low] = ADC0L;
      000531 E5 11            [12] 2938 	mov	a,_le_adc0_PARM_4
      000533 24 25            [12] 2939 	add	a,#_saida
      000535 F8               [12] 2940 	mov	r0,a
      000536 A6 BE            [24] 2941 	mov	@r0,_ADC0L
                           00048D  2942 	C$sensores.c$129$1$75 ==.
                           00048D  2943 	XG$le_adc0$0$0 ==.
      000538 22               [24] 2944 	ret
                                   2945 ;------------------------------------------------------------
                                   2946 ;Allocation info for local variables in function 'le_voltagem'
                                   2947 ;------------------------------------------------------------
                                   2948 ;ganho                     Allocated with name '_le_voltagem_PARM_2'
                                   2949 ;cod                       Allocated to registers r6 r7 
                                   2950 ;g                         Allocated to registers r2 r3 r4 r5 
                                   2951 ;------------------------------------------------------------
                           00048E  2952 	G$le_voltagem$0$0 ==.
                           00048E  2953 	C$sensores.c$131$1$75 ==.
                                   2954 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:131: float le_voltagem(unsigned int cod, unsigned char ganho){
                                   2955 ;	-----------------------------------------
                                   2956 ;	 function le_voltagem
                                   2957 ;	-----------------------------------------
      000539                       2958 _le_voltagem:
      000539 AE 82            [24] 2959 	mov	r6,dpl
      00053B AF 83            [24] 2960 	mov	r7,dph
                           000492  2961 	C$sensores.c$136$1$77 ==.
                                   2962 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:136: if(ganho == GAIN01) g = 1;
      00053D E5 2B            [12] 2963 	mov	a,_le_voltagem_PARM_2
      00053F 70 08            [24] 2964 	jnz	00114$
      000541 FA               [12] 2965 	mov	r2,a
      000542 FB               [12] 2966 	mov	r3,a
      000543 7C 80            [12] 2967 	mov	r4,#0x80
      000545 7D 3F            [12] 2968 	mov	r5,#0x3f
      000547 80 44            [24] 2969 	sjmp	00115$
      000549                       2970 00114$:
                           00049E  2971 	C$sensores.c$137$1$77 ==.
                                   2972 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:137: else if(ganho == GAIN02) g = 2;
      000549 74 01            [12] 2973 	mov	a,#0x01
      00054B B5 2B 0A         [24] 2974 	cjne	a,_le_voltagem_PARM_2,00111$
      00054E 7A 00            [12] 2975 	mov	r2,#0x00
      000550 7B 00            [12] 2976 	mov	r3,#0x00
      000552 7C 00            [12] 2977 	mov	r4,#0x00
      000554 7D 40            [12] 2978 	mov	r5,#0x40
      000556 80 35            [24] 2979 	sjmp	00115$
      000558                       2980 00111$:
                           0004AD  2981 	C$sensores.c$138$1$77 ==.
                                   2982 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:138: else if(ganho == GAIN04) g = 4;
      000558 74 02            [12] 2983 	mov	a,#0x02
      00055A B5 2B 0A         [24] 2984 	cjne	a,_le_voltagem_PARM_2,00108$
      00055D 7A 00            [12] 2985 	mov	r2,#0x00
      00055F 7B 00            [12] 2986 	mov	r3,#0x00
      000561 7C 80            [12] 2987 	mov	r4,#0x80
      000563 7D 40            [12] 2988 	mov	r5,#0x40
      000565 80 26            [24] 2989 	sjmp	00115$
      000567                       2990 00108$:
                           0004BC  2991 	C$sensores.c$139$1$77 ==.
                                   2992 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:139: else if(ganho == GAIN08) g = 8;
      000567 74 03            [12] 2993 	mov	a,#0x03
      000569 B5 2B 0A         [24] 2994 	cjne	a,_le_voltagem_PARM_2,00105$
      00056C 7A 00            [12] 2995 	mov	r2,#0x00
      00056E 7B 00            [12] 2996 	mov	r3,#0x00
      000570 7C 00            [12] 2997 	mov	r4,#0x00
      000572 7D 41            [12] 2998 	mov	r5,#0x41
      000574 80 17            [24] 2999 	sjmp	00115$
      000576                       3000 00105$:
                           0004CB  3001 	C$sensores.c$140$1$77 ==.
                                   3002 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:140: else if(ganho == GAIN16) g = 16;
      000576 74 04            [12] 3003 	mov	a,#0x04
      000578 B5 2B 0A         [24] 3004 	cjne	a,_le_voltagem_PARM_2,00102$
      00057B 7A 00            [12] 3005 	mov	r2,#0x00
      00057D 7B 00            [12] 3006 	mov	r3,#0x00
      00057F 7C 80            [12] 3007 	mov	r4,#0x80
      000581 7D 41            [12] 3008 	mov	r5,#0x41
      000583 80 08            [24] 3009 	sjmp	00115$
      000585                       3010 00102$:
                           0004DA  3011 	C$sensores.c$141$1$77 ==.
                                   3012 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:141: else g = 0.5;
      000585 7A 00            [12] 3013 	mov	r2,#0x00
      000587 7B 00            [12] 3014 	mov	r3,#0x00
      000589 7C 00            [12] 3015 	mov	r4,#0x00
      00058B 7D 3F            [12] 3016 	mov	r5,#0x3f
      00058D                       3017 00115$:
                           0004E2  3018 	C$sensores.c$143$1$77 ==.
                                   3019 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:143: return (cod*VREF_DIV_P2N/g);
      00058D 8E 82            [24] 3020 	mov	dpl,r6
      00058F 8F 83            [24] 3021 	mov	dph,r7
      000591 C0 05            [24] 3022 	push	ar5
      000593 C0 04            [24] 3023 	push	ar4
      000595 C0 03            [24] 3024 	push	ar3
      000597 C0 02            [24] 3025 	push	ar2
      000599 12 14 50         [24] 3026 	lcall	___uint2fs
      00059C A8 82            [24] 3027 	mov	r0,dpl
      00059E A9 83            [24] 3028 	mov	r1,dph
      0005A0 AE F0            [24] 3029 	mov	r6,b
      0005A2 FF               [12] 3030 	mov	r7,a
      0005A3 C0 00            [24] 3031 	push	ar0
      0005A5 C0 01            [24] 3032 	push	ar1
      0005A7 C0 06            [24] 3033 	push	ar6
      0005A9 C0 07            [24] 3034 	push	ar7
      0005AB 90 85 1F         [24] 3035 	mov	dptr,#0x851f
      0005AE 75 F0 1B         [24] 3036 	mov	b,#0x1b
      0005B1 74 3A            [12] 3037 	mov	a,#0x3a
      0005B3 12 12 90         [24] 3038 	lcall	___fsmul
      0005B6 A8 82            [24] 3039 	mov	r0,dpl
      0005B8 A9 83            [24] 3040 	mov	r1,dph
      0005BA AE F0            [24] 3041 	mov	r6,b
      0005BC FF               [12] 3042 	mov	r7,a
      0005BD E5 81            [12] 3043 	mov	a,sp
      0005BF 24 FC            [12] 3044 	add	a,#0xfc
      0005C1 F5 81            [12] 3045 	mov	sp,a
      0005C3 D0 02            [24] 3046 	pop	ar2
      0005C5 D0 03            [24] 3047 	pop	ar3
      0005C7 D0 04            [24] 3048 	pop	ar4
      0005C9 D0 05            [24] 3049 	pop	ar5
      0005CB C0 02            [24] 3050 	push	ar2
      0005CD C0 03            [24] 3051 	push	ar3
      0005CF C0 04            [24] 3052 	push	ar4
      0005D1 C0 05            [24] 3053 	push	ar5
      0005D3 88 82            [24] 3054 	mov	dpl,r0
      0005D5 89 83            [24] 3055 	mov	dph,r1
      0005D7 8E F0            [24] 3056 	mov	b,r6
      0005D9 EF               [12] 3057 	mov	a,r7
      0005DA 12 14 AB         [24] 3058 	lcall	___fsdiv
      0005DD AC 82            [24] 3059 	mov	r4,dpl
      0005DF AD 83            [24] 3060 	mov	r5,dph
      0005E1 AE F0            [24] 3061 	mov	r6,b
      0005E3 FF               [12] 3062 	mov	r7,a
      0005E4 E5 81            [12] 3063 	mov	a,sp
      0005E6 24 FC            [12] 3064 	add	a,#0xfc
      0005E8 F5 81            [12] 3065 	mov	sp,a
      0005EA 8C 82            [24] 3066 	mov	dpl,r4
      0005EC 8D 83            [24] 3067 	mov	dph,r5
      0005EE 8E F0            [24] 3068 	mov	b,r6
      0005F0 EF               [12] 3069 	mov	a,r7
                           000546  3070 	C$sensores.c$144$1$77 ==.
                           000546  3071 	XG$le_voltagem$0$0 ==.
      0005F1 22               [24] 3072 	ret
                                   3073 ;------------------------------------------------------------
                                   3074 ;Allocation info for local variables in function 'le_sensores'
                                   3075 ;------------------------------------------------------------
                           000547  3076 	G$le_sensores$0$0 ==.
                           000547  3077 	C$sensores.c$146$1$77 ==.
                                   3078 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:146: void le_sensores(void){
                                   3079 ;	-----------------------------------------
                                   3080 ;	 function le_sensores
                                   3081 ;	-----------------------------------------
      0005F2                       3082 _le_sensores:
                           000547  3083 	C$sensores.c$149$1$79 ==.
                                   3084 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:149: le_dht11();
      0005F2 12 04 AF         [24] 3085 	lcall	_le_dht11
                           00054A  3086 	C$sensores.c$150$1$79 ==.
                                   3087 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:150: le_adc0(AIN0_1, GAIN_5, LDR_HI, LDR_LO);
      0005F5 75 0F 06         [24] 3088 	mov	_le_adc0_PARM_2,#0x06
      0005F8 75 10 04         [24] 3089 	mov	_le_adc0_PARM_3,#0x04
      0005FB 75 11 03         [24] 3090 	mov	_le_adc0_PARM_4,#0x03
      0005FE 75 82 01         [24] 3091 	mov	dpl,#0x01
      000601 12 05 18         [24] 3092 	lcall	_le_adc0
                           000559  3093 	C$sensores.c$151$1$79 ==.
                                   3094 ;	C:\Users\202019050584\Desktop\Trabalho\/sensores.c:151: saida[B_CHUVA] = (unsigned char)MHRD;
      000604 A2 86            [12] 3095 	mov	c,_P0_6
      000606 E4               [12] 3096 	clr	a
      000607 33               [12] 3097 	rlc	a
      000608 FF               [12] 3098 	mov	r7,a
      000609 8F 2A            [24] 3099 	mov	(_saida + 0x0005),r7
                           000560  3100 	C$sensores.c$152$1$79 ==.
                           000560  3101 	XG$le_sensores$0$0 ==.
      00060B 22               [24] 3102 	ret
                                   3103 ;------------------------------------------------------------
                                   3104 ;Allocation info for local variables in function 'esc_RAM_SPI'
                                   3105 ;------------------------------------------------------------
                                   3106 ;dado                      Allocated with name '_esc_RAM_SPI_PARM_2'
                                   3107 ;end                       Allocated to registers r6 r7 
                                   3108 ;end_l                     Allocated to registers r5 
                                   3109 ;end_h                     Allocated to registers r7 
                                   3110 ;------------------------------------------------------------
                           000561  3111 	G$esc_RAM_SPI$0$0 ==.
                           000561  3112 	C$ram_spi.c$17$1$79 ==.
                                   3113 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:17: void esc_RAM_SPI(unsigned int end, unsigned char dado){
                                   3114 ;	-----------------------------------------
                                   3115 ;	 function esc_RAM_SPI
                                   3116 ;	-----------------------------------------
      00060C                       3117 _esc_RAM_SPI:
      00060C AE 82            [24] 3118 	mov	r6,dpl
      00060E AF 83            [24] 3119 	mov	r7,dph
                           000565  3120 	C$ram_spi.c$18$1$79 ==.
                                   3121 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:18: unsigned char end_l = end, end_h = end>>8;
      000610 8E 05            [24] 3122 	mov	ar5,r6
                           000567  3123 	C$ram_spi.c$20$1$81 ==.
                                   3124 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:20: CS = LO;
      000612 C2 A3            [12] 3125 	clr	_P2_3
                           000569  3126 	C$ram_spi.c$22$1$81 ==.
                                   3127 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:22: SPI0DAT = 0x02;
      000614 75 9B 02         [24] 3128 	mov	_SPI0DAT,#0x02
                           00056C  3129 	C$ram_spi.c$23$1$81 ==.
                                   3130 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:23: while(TXBMT==0); // Espera o shift dos 16 bits serem shiftados
      000617                       3131 00101$:
      000617 30 F9 FD         [24] 3132 	jnb	_TXBMT,00101$
                           00056F  3133 	C$ram_spi.c$25$1$81 ==.
                                   3134 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:25: SPI0DAT = end_h;
      00061A 8F 9B            [24] 3135 	mov	_SPI0DAT,r7
                           000571  3136 	C$ram_spi.c$26$1$81 ==.
                                   3137 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:26: while(TXBMT==0);
      00061C                       3138 00104$:
      00061C 30 F9 FD         [24] 3139 	jnb	_TXBMT,00104$
                           000574  3140 	C$ram_spi.c$28$1$81 ==.
                                   3141 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:28: SPI0DAT = end_l;
      00061F 8D 9B            [24] 3142 	mov	_SPI0DAT,r5
                           000576  3143 	C$ram_spi.c$29$1$81 ==.
                                   3144 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:29: while(TXBMT==0);
      000621                       3145 00107$:
      000621 30 F9 FD         [24] 3146 	jnb	_TXBMT,00107$
                           000579  3147 	C$ram_spi.c$31$1$81 ==.
                                   3148 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:31: SPI0DAT = dado;
      000624 85 0F 9B         [24] 3149 	mov	_SPI0DAT,_esc_RAM_SPI_PARM_2
                           00057C  3150 	C$ram_spi.c$32$1$81 ==.
                                   3151 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:32: while(TXBMT==0);
      000627                       3152 00110$:
      000627 30 F9 FD         [24] 3153 	jnb	_TXBMT,00110$
                           00057F  3154 	C$ram_spi.c$34$1$81 ==.
                                   3155 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:34: SPIF = 0; // Reseta valor para receber bit flag
      00062A C2 FF            [12] 3156 	clr	_SPIF
                           000581  3157 	C$ram_spi.c$35$1$81 ==.
                                   3158 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:35: while(SPIF==0); // Aguarda a sinalizacao do bit flag do fim da instrucao
      00062C                       3159 00113$:
                           000581  3160 	C$ram_spi.c$36$1$81 ==.
                                   3161 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:36: SPIF = 0; // Reseta valor para receber bit flag
      00062C 10 FF 02         [24] 3162 	jbc	_SPIF,00152$
      00062F 80 FB            [24] 3163 	sjmp	00113$
      000631                       3164 00152$:
                           000586  3165 	C$ram_spi.c$38$1$81 ==.
                                   3166 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:38: CS = 1;
      000631 D2 A3            [12] 3167 	setb	_P2_3
                           000588  3168 	C$ram_spi.c$39$1$81 ==.
                           000588  3169 	XG$esc_RAM_SPI$0$0 ==.
      000633 22               [24] 3170 	ret
                                   3171 ;------------------------------------------------------------
                                   3172 ;Allocation info for local variables in function 'le_RAM_SPI'
                                   3173 ;------------------------------------------------------------
                                   3174 ;end                       Allocated to registers r6 r7 
                                   3175 ;end_l                     Allocated to registers r5 
                                   3176 ;end_h                     Allocated to registers r7 
                                   3177 ;------------------------------------------------------------
                           000589  3178 	G$le_RAM_SPI$0$0 ==.
                           000589  3179 	C$ram_spi.c$41$1$81 ==.
                                   3180 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:41: unsigned char le_RAM_SPI(unsigned int end){
                                   3181 ;	-----------------------------------------
                                   3182 ;	 function le_RAM_SPI
                                   3183 ;	-----------------------------------------
      000634                       3184 _le_RAM_SPI:
      000634 AE 82            [24] 3185 	mov	r6,dpl
      000636 AF 83            [24] 3186 	mov	r7,dph
                           00058D  3187 	C$ram_spi.c$42$1$81 ==.
                                   3188 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:42: unsigned char end_l = end, end_h = end>>8;
      000638 8E 05            [24] 3189 	mov	ar5,r6
                           00058F  3190 	C$ram_spi.c$44$1$83 ==.
                                   3191 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:44: CS = LO;
      00063A C2 A3            [12] 3192 	clr	_P2_3
                           000591  3193 	C$ram_spi.c$46$1$83 ==.
                                   3194 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:46: SPI0DAT = 0x03; 
      00063C 75 9B 03         [24] 3195 	mov	_SPI0DAT,#0x03
                           000594  3196 	C$ram_spi.c$47$1$83 ==.
                                   3197 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:47: while(TXBMT==0); // Espera o shift dos 16 bits serem shiftados
      00063F                       3198 00101$:
      00063F 30 F9 FD         [24] 3199 	jnb	_TXBMT,00101$
                           000597  3200 	C$ram_spi.c$49$1$83 ==.
                                   3201 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:49: SPI0DAT = end_h;
      000642 8F 9B            [24] 3202 	mov	_SPI0DAT,r7
                           000599  3203 	C$ram_spi.c$50$1$83 ==.
                                   3204 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:50: while(TXBMT==0);
      000644                       3205 00104$:
      000644 30 F9 FD         [24] 3206 	jnb	_TXBMT,00104$
                           00059C  3207 	C$ram_spi.c$52$1$83 ==.
                                   3208 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:52: SPI0DAT = end_l;
      000647 8D 9B            [24] 3209 	mov	_SPI0DAT,r5
                           00059E  3210 	C$ram_spi.c$53$1$83 ==.
                                   3211 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:53: while(TXBMT==0);
      000649                       3212 00107$:
      000649 30 F9 FD         [24] 3213 	jnb	_TXBMT,00107$
                           0005A1  3214 	C$ram_spi.c$55$1$83 ==.
                                   3215 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:55: SPI0DAT = 0x00; // Garantir que o dado foi zerado. Limpar a memoria de dados flash
      00064C 75 9B 00         [24] 3216 	mov	_SPI0DAT,#0x00
                           0005A4  3217 	C$ram_spi.c$56$1$83 ==.
                                   3218 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:56: while(TXBMT==0);
      00064F                       3219 00110$:
      00064F 30 F9 FD         [24] 3220 	jnb	_TXBMT,00110$
                           0005A7  3221 	C$ram_spi.c$58$1$83 ==.
                                   3222 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:58: SPIF = 0;
      000652 C2 FF            [12] 3223 	clr	_SPIF
                           0005A9  3224 	C$ram_spi.c$59$1$83 ==.
                                   3225 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:59: while(SPIF==0);
      000654                       3226 00113$:
                           0005A9  3227 	C$ram_spi.c$60$1$83 ==.
                                   3228 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:60: SPIF = 0;
      000654 10 FF 02         [24] 3229 	jbc	_SPIF,00152$
      000657 80 FB            [24] 3230 	sjmp	00113$
      000659                       3231 00152$:
                           0005AE  3232 	C$ram_spi.c$62$1$83 ==.
                                   3233 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:62: CS = 1;
      000659 D2 A3            [12] 3234 	setb	_P2_3
                           0005B0  3235 	C$ram_spi.c$64$1$83 ==.
                                   3236 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:64: return SPI0DAT;
      00065B 85 9B 82         [24] 3237 	mov	dpl,_SPI0DAT
                           0005B3  3238 	C$ram_spi.c$65$1$83 ==.
                           0005B3  3239 	XG$le_RAM_SPI$0$0 ==.
      00065E 22               [24] 3240 	ret
                                   3241 ;------------------------------------------------------------
                                   3242 ;Allocation info for local variables in function 'verifica_RAM_SPI'
                                   3243 ;------------------------------------------------------------
                                   3244 ;i                         Allocated to registers r6 r7 
                                   3245 ;aux                       Allocated to registers r3 
                                   3246 ;------------------------------------------------------------
                           0005B4  3247 	G$verifica_RAM_SPI$0$0 ==.
                           0005B4  3248 	C$ram_spi.c$67$1$83 ==.
                                   3249 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:67: unsigned char verifica_RAM_SPI(void){
                                   3250 ;	-----------------------------------------
                                   3251 ;	 function verifica_RAM_SPI
                                   3252 ;	-----------------------------------------
      00065F                       3253 _verifica_RAM_SPI:
                           0005B4  3254 	C$ram_spi.c$73$1$85 ==.
                                   3255 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:73: for(i=0; i<8192; i++){
      00065F 7E 00            [12] 3256 	mov	r6,#0x00
      000661 7F 00            [12] 3257 	mov	r7,#0x00
      000663 7C 00            [12] 3258 	mov	r4,#0x00
      000665 7D 00            [12] 3259 	mov	r5,#0x00
      000667                       3260 00104$:
                           0005BC  3261 	C$ram_spi.c$74$2$86 ==.
                                   3262 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:74: esc_RAM_SPI(i, 170);
      000667 75 0F AA         [24] 3263 	mov	_esc_RAM_SPI_PARM_2,#0xaa
      00066A 8C 82            [24] 3264 	mov	dpl,r4
      00066C 8D 83            [24] 3265 	mov	dph,r5
      00066E C0 07            [24] 3266 	push	ar7
      000670 C0 06            [24] 3267 	push	ar6
      000672 C0 05            [24] 3268 	push	ar5
      000674 C0 04            [24] 3269 	push	ar4
      000676 12 06 0C         [24] 3270 	lcall	_esc_RAM_SPI
      000679 D0 04            [24] 3271 	pop	ar4
      00067B D0 05            [24] 3272 	pop	ar5
                           0005D2  3273 	C$ram_spi.c$75$2$86 ==.
                                   3274 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:75: aux = le_RAM_SPI(i);
      00067D 8C 82            [24] 3275 	mov	dpl,r4
      00067F 8D 83            [24] 3276 	mov	dph,r5
      000681 C0 05            [24] 3277 	push	ar5
      000683 C0 04            [24] 3278 	push	ar4
      000685 12 06 34         [24] 3279 	lcall	_le_RAM_SPI
      000688 AB 82            [24] 3280 	mov	r3,dpl
      00068A D0 04            [24] 3281 	pop	ar4
      00068C D0 05            [24] 3282 	pop	ar5
      00068E D0 06            [24] 3283 	pop	ar6
      000690 D0 07            [24] 3284 	pop	ar7
                           0005E7  3285 	C$ram_spi.c$77$2$86 ==.
                                   3286 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:77: if(aux != 170){
      000692 BB AA 02         [24] 3287 	cjne	r3,#0xaa,00117$
      000695 80 1A            [24] 3288 	sjmp	00102$
      000697                       3289 00117$:
                           0005EC  3290 	C$ram_spi.c$78$3$87 ==.
                                   3291 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:78: printf_fast_f("\x02 ERRO: mem=%05d",i);
      000697 C0 06            [24] 3292 	push	ar6
      000699 C0 07            [24] 3293 	push	ar7
      00069B 74 86            [12] 3294 	mov	a,#___str_0
      00069D C0 E0            [24] 3295 	push	acc
      00069F 74 17            [12] 3296 	mov	a,#(___str_0 >> 8)
      0006A1 C0 E0            [24] 3297 	push	acc
      0006A3 12 0E 0F         [24] 3298 	lcall	_printf_fast_f
      0006A6 E5 81            [12] 3299 	mov	a,sp
      0006A8 24 FC            [12] 3300 	add	a,#0xfc
      0006AA F5 81            [12] 3301 	mov	sp,a
                           000601  3302 	C$ram_spi.c$79$3$87 ==.
                                   3303 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:79: return 0; //erro em um endereco
      0006AC 75 82 00         [24] 3304 	mov	dpl,#0x00
      0006AF 80 2E            [24] 3305 	sjmp	00106$
      0006B1                       3306 00102$:
                           000606  3307 	C$ram_spi.c$81$2$86 ==.
                                   3308 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:81: printf_fast_f("\x02 i = %05d",i);
      0006B1 C0 05            [24] 3309 	push	ar5
      0006B3 C0 04            [24] 3310 	push	ar4
      0006B5 C0 04            [24] 3311 	push	ar4
      0006B7 C0 05            [24] 3312 	push	ar5
      0006B9 74 97            [12] 3313 	mov	a,#___str_1
      0006BB C0 E0            [24] 3314 	push	acc
      0006BD 74 17            [12] 3315 	mov	a,#(___str_1 >> 8)
      0006BF C0 E0            [24] 3316 	push	acc
      0006C1 12 0E 0F         [24] 3317 	lcall	_printf_fast_f
      0006C4 E5 81            [12] 3318 	mov	a,sp
      0006C6 24 FC            [12] 3319 	add	a,#0xfc
      0006C8 F5 81            [12] 3320 	mov	sp,a
      0006CA D0 04            [24] 3321 	pop	ar4
      0006CC D0 05            [24] 3322 	pop	ar5
                           000623  3323 	C$ram_spi.c$73$1$85 ==.
                                   3324 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:73: for(i=0; i<8192; i++){
      0006CE 0C               [12] 3325 	inc	r4
      0006CF BC 00 01         [24] 3326 	cjne	r4,#0x00,00118$
      0006D2 0D               [12] 3327 	inc	r5
      0006D3                       3328 00118$:
      0006D3 8C 06            [24] 3329 	mov	ar6,r4
      0006D5 8D 07            [24] 3330 	mov	ar7,r5
      0006D7 74 E0            [12] 3331 	mov	a,#0x100 - 0x20
      0006D9 2D               [12] 3332 	add	a,r5
      0006DA 50 8B            [24] 3333 	jnc	00104$
                           000631  3334 	C$ram_spi.c$84$1$85 ==.
                                   3335 ;	C:\Users\202019050584\Desktop\Trabalho\/ram_spi.c:84: return 1; //tudo certo
      0006DC 75 82 01         [24] 3336 	mov	dpl,#0x01
      0006DF                       3337 00106$:
                           000634  3338 	C$ram_spi.c$85$1$85 ==.
                           000634  3339 	XG$verifica_RAM_SPI$0$0 ==.
      0006DF 22               [24] 3340 	ret
                                   3341 ;------------------------------------------------------------
                                   3342 ;Allocation info for local variables in function 'print_relogio_terminal'
                                   3343 ;------------------------------------------------------------
                                   3344 ;sloc0                     Allocated with name '_print_relogio_terminal_sloc0_1_0'
                                   3345 ;sloc1                     Allocated with name '_print_relogio_terminal_sloc1_1_0'
                                   3346 ;sloc2                     Allocated with name '_print_relogio_terminal_sloc2_1_0'
                                   3347 ;------------------------------------------------------------
                           000635  3348 	G$print_relogio_terminal$0$0 ==.
                           000635  3349 	C$tempo.c$18$1$85 ==.
                                   3350 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:18: void print_relogio_terminal(void){
                                   3351 ;	-----------------------------------------
                                   3352 ;	 function print_relogio_terminal
                                   3353 ;	-----------------------------------------
      0006E0                       3354 _print_relogio_terminal:
                           000635  3355 	C$tempo.c$21$1$89 ==.
                                   3356 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:21: printf_fast_f(" %02d/%02d/2%03d | %02d:%02d:%02d |", relogio[DIA]+1, relogio[MES]+1, relogio[ANO], relogio[HOR], relogio[MIN], relogio[SEG]);
      0006E0 AE 33            [24] 3357 	mov	r6,(_relogio + 0x0005)
      0006E2 7F 00            [12] 3358 	mov	r7,#0x00
      0006E4 AC 32            [24] 3359 	mov	r4,(_relogio + 0x0004)
      0006E6 7D 00            [12] 3360 	mov	r5,#0x00
      0006E8 85 31 35         [24] 3361 	mov	_print_relogio_terminal_sloc0_1_0,(_relogio + 0x0003)
                                   3362 ;	1-genFromRTrack replaced	mov	(_print_relogio_terminal_sloc0_1_0 + 1),#0x00
      0006EB 8F 36            [24] 3363 	mov	(_print_relogio_terminal_sloc0_1_0 + 1),r7
      0006ED 85 30 37         [24] 3364 	mov	_print_relogio_terminal_sloc1_1_0,(_relogio + 0x0002)
                                   3365 ;	1-genFromRTrack replaced	mov	(_print_relogio_terminal_sloc1_1_0 + 1),#0x00
      0006F0 8F 38            [24] 3366 	mov	(_print_relogio_terminal_sloc1_1_0 + 1),r7
      0006F2 AA 2F            [24] 3367 	mov	r2,(_relogio + 0x0001)
      0006F4 7B 00            [12] 3368 	mov	r3,#0x00
      0006F6 74 01            [12] 3369 	mov	a,#0x01
      0006F8 2A               [12] 3370 	add	a,r2
      0006F9 F5 39            [12] 3371 	mov	_print_relogio_terminal_sloc2_1_0,a
      0006FB E4               [12] 3372 	clr	a
      0006FC 3B               [12] 3373 	addc	a,r3
      0006FD F5 3A            [12] 3374 	mov	(_print_relogio_terminal_sloc2_1_0 + 1),a
      0006FF AA 2E            [24] 3375 	mov	r2,_relogio
      000701 7B 00            [12] 3376 	mov	r3,#0x00
      000703 0A               [12] 3377 	inc	r2
      000704 BA 00 01         [24] 3378 	cjne	r2,#0x00,00103$
      000707 0B               [12] 3379 	inc	r3
      000708                       3380 00103$:
      000708 C0 06            [24] 3381 	push	ar6
      00070A C0 07            [24] 3382 	push	ar7
      00070C C0 04            [24] 3383 	push	ar4
      00070E C0 05            [24] 3384 	push	ar5
      000710 C0 35            [24] 3385 	push	_print_relogio_terminal_sloc0_1_0
      000712 C0 36            [24] 3386 	push	(_print_relogio_terminal_sloc0_1_0 + 1)
      000714 C0 37            [24] 3387 	push	_print_relogio_terminal_sloc1_1_0
      000716 C0 38            [24] 3388 	push	(_print_relogio_terminal_sloc1_1_0 + 1)
      000718 C0 39            [24] 3389 	push	_print_relogio_terminal_sloc2_1_0
      00071A C0 3A            [24] 3390 	push	(_print_relogio_terminal_sloc2_1_0 + 1)
      00071C C0 02            [24] 3391 	push	ar2
      00071E C0 03            [24] 3392 	push	ar3
      000720 74 A2            [12] 3393 	mov	a,#___str_2
      000722 C0 E0            [24] 3394 	push	acc
      000724 74 17            [12] 3395 	mov	a,#(___str_2 >> 8)
      000726 C0 E0            [24] 3396 	push	acc
      000728 12 0E 0F         [24] 3397 	lcall	_printf_fast_f
      00072B E5 81            [12] 3398 	mov	a,sp
      00072D 24 F2            [12] 3399 	add	a,#0xf2
      00072F F5 81            [12] 3400 	mov	sp,a
                           000686  3401 	C$tempo.c$22$1$89 ==.
                           000686  3402 	XG$print_relogio_terminal$0$0 ==.
      000731 22               [24] 3403 	ret
                                   3404 ;------------------------------------------------------------
                                   3405 ;Allocation info for local variables in function 'print_relogio_glcd'
                                   3406 ;------------------------------------------------------------
                                   3407 ;sloc0                     Allocated with name '_print_relogio_glcd_sloc0_1_0'
                                   3408 ;sloc1                     Allocated with name '_print_relogio_glcd_sloc1_1_0'
                                   3409 ;sloc2                     Allocated with name '_print_relogio_glcd_sloc2_1_0'
                                   3410 ;------------------------------------------------------------
                           000687  3411 	G$print_relogio_glcd$0$0 ==.
                           000687  3412 	C$tempo.c$24$1$89 ==.
                                   3413 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:24: void print_relogio_glcd(void){
                                   3414 ;	-----------------------------------------
                                   3415 ;	 function print_relogio_glcd
                                   3416 ;	-----------------------------------------
      000732                       3417 _print_relogio_glcd:
                           000687  3418 	C$tempo.c$27$1$91 ==.
                                   3419 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:27: printf_fast_f("\x01 %02d/%02d/2%03d \x02 %02d:%02d:%02d\n", relogio[DIA]+1, relogio[MES]+1, relogio[ANO], relogio[HOR], relogio[MIN], relogio[SEG]);
      000732 AE 33            [24] 3420 	mov	r6,(_relogio + 0x0005)
      000734 7F 00            [12] 3421 	mov	r7,#0x00
      000736 AC 32            [24] 3422 	mov	r4,(_relogio + 0x0004)
      000738 7D 00            [12] 3423 	mov	r5,#0x00
      00073A 85 31 3B         [24] 3424 	mov	_print_relogio_glcd_sloc0_1_0,(_relogio + 0x0003)
                                   3425 ;	1-genFromRTrack replaced	mov	(_print_relogio_glcd_sloc0_1_0 + 1),#0x00
      00073D 8F 3C            [24] 3426 	mov	(_print_relogio_glcd_sloc0_1_0 + 1),r7
      00073F 85 30 3D         [24] 3427 	mov	_print_relogio_glcd_sloc1_1_0,(_relogio + 0x0002)
                                   3428 ;	1-genFromRTrack replaced	mov	(_print_relogio_glcd_sloc1_1_0 + 1),#0x00
      000742 8F 3E            [24] 3429 	mov	(_print_relogio_glcd_sloc1_1_0 + 1),r7
      000744 AA 2F            [24] 3430 	mov	r2,(_relogio + 0x0001)
      000746 7B 00            [12] 3431 	mov	r3,#0x00
      000748 74 01            [12] 3432 	mov	a,#0x01
      00074A 2A               [12] 3433 	add	a,r2
      00074B F5 3F            [12] 3434 	mov	_print_relogio_glcd_sloc2_1_0,a
      00074D E4               [12] 3435 	clr	a
      00074E 3B               [12] 3436 	addc	a,r3
      00074F F5 40            [12] 3437 	mov	(_print_relogio_glcd_sloc2_1_0 + 1),a
      000751 AA 2E            [24] 3438 	mov	r2,_relogio
      000753 7B 00            [12] 3439 	mov	r3,#0x00
      000755 0A               [12] 3440 	inc	r2
      000756 BA 00 01         [24] 3441 	cjne	r2,#0x00,00103$
      000759 0B               [12] 3442 	inc	r3
      00075A                       3443 00103$:
      00075A C0 06            [24] 3444 	push	ar6
      00075C C0 07            [24] 3445 	push	ar7
      00075E C0 04            [24] 3446 	push	ar4
      000760 C0 05            [24] 3447 	push	ar5
      000762 C0 3B            [24] 3448 	push	_print_relogio_glcd_sloc0_1_0
      000764 C0 3C            [24] 3449 	push	(_print_relogio_glcd_sloc0_1_0 + 1)
      000766 C0 3D            [24] 3450 	push	_print_relogio_glcd_sloc1_1_0
      000768 C0 3E            [24] 3451 	push	(_print_relogio_glcd_sloc1_1_0 + 1)
      00076A C0 3F            [24] 3452 	push	_print_relogio_glcd_sloc2_1_0
      00076C C0 40            [24] 3453 	push	(_print_relogio_glcd_sloc2_1_0 + 1)
      00076E C0 02            [24] 3454 	push	ar2
      000770 C0 03            [24] 3455 	push	ar3
      000772 74 C6            [12] 3456 	mov	a,#___str_3
      000774 C0 E0            [24] 3457 	push	acc
      000776 74 17            [12] 3458 	mov	a,#(___str_3 >> 8)
      000778 C0 E0            [24] 3459 	push	acc
      00077A 12 0E 0F         [24] 3460 	lcall	_printf_fast_f
      00077D E5 81            [12] 3461 	mov	a,sp
      00077F 24 F2            [12] 3462 	add	a,#0xf2
      000781 F5 81            [12] 3463 	mov	sp,a
                           0006D8  3464 	C$tempo.c$28$1$91 ==.
                           0006D8  3465 	XG$print_relogio_glcd$0$0 ==.
      000783 22               [24] 3466 	ret
                                   3467 ;------------------------------------------------------------
                                   3468 ;Allocation info for local variables in function 'ano_bissexto'
                                   3469 ;------------------------------------------------------------
                           0006D9  3470 	G$ano_bissexto$0$0 ==.
                           0006D9  3471 	C$tempo.c$30$1$91 ==.
                                   3472 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:30: unsigned char ano_bissexto(void){
                                   3473 ;	-----------------------------------------
                                   3474 ;	 function ano_bissexto
                                   3475 ;	-----------------------------------------
      000784                       3476 _ano_bissexto:
                           0006D9  3477 	C$tempo.c$33$1$93 ==.
                                   3478 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:33: if(relogio[ANO]%4==0) return 1;
      000784 E5 30            [12] 3479 	mov	a,(_relogio + 0x0002)
      000786 54 03            [12] 3480 	anl	a,#0x03
      000788 60 02            [24] 3481 	jz	00109$
      00078A 80 05            [24] 3482 	sjmp	00102$
      00078C                       3483 00109$:
      00078C 75 82 01         [24] 3484 	mov	dpl,#0x01
      00078F 80 03            [24] 3485 	sjmp	00103$
      000791                       3486 00102$:
                           0006E6  3487 	C$tempo.c$34$1$93 ==.
                                   3488 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:34: return 0;
      000791 75 82 00         [24] 3489 	mov	dpl,#0x00
      000794                       3490 00103$:
                           0006E9  3491 	C$tempo.c$35$1$93 ==.
                           0006E9  3492 	XG$ano_bissexto$0$0 ==.
      000794 22               [24] 3493 	ret
                                   3494 ;------------------------------------------------------------
                                   3495 ;Allocation info for local variables in function 'ini_relogio'
                                   3496 ;------------------------------------------------------------
                                   3497 ;mes                       Allocated with name '_ini_relogio_PARM_2'
                                   3498 ;ano                       Allocated with name '_ini_relogio_PARM_3'
                                   3499 ;hora                      Allocated with name '_ini_relogio_PARM_4'
                                   3500 ;minuto                    Allocated with name '_ini_relogio_PARM_5'
                                   3501 ;segundo                   Allocated with name '_ini_relogio_PARM_6'
                                   3502 ;dia                       Allocated to registers r7 
                                   3503 ;------------------------------------------------------------
                           0006EA  3504 	G$ini_relogio$0$0 ==.
                           0006EA  3505 	C$tempo.c$37$1$93 ==.
                                   3506 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:37: void ini_relogio(unsigned char dia, unsigned char mes, unsigned char ano, unsigned char hora, unsigned char minuto, unsigned char segundo){
                                   3507 ;	-----------------------------------------
                                   3508 ;	 function ini_relogio
                                   3509 ;	-----------------------------------------
      000795                       3510 _ini_relogio:
                           0006EA  3511 	C$tempo.c$40$1$95 ==.
                                   3512 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:40: relogio[DIA] = dia-1;
      000795 E5 82            [12] 3513 	mov	a,dpl
      000797 14               [12] 3514 	dec	a
      000798 F5 2E            [12] 3515 	mov	_relogio,a
                           0006EF  3516 	C$tempo.c$41$1$95 ==.
                                   3517 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:41: relogio[MES] = mes-1;
      00079A E5 0F            [12] 3518 	mov	a,_ini_relogio_PARM_2
      00079C 14               [12] 3519 	dec	a
      00079D F5 2F            [12] 3520 	mov	(_relogio + 0x0001),a
                           0006F4  3521 	C$tempo.c$42$1$95 ==.
                                   3522 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:42: relogio[ANO] = ano;
      00079F 85 10 30         [24] 3523 	mov	(_relogio + 0x0002),_ini_relogio_PARM_3
                           0006F7  3524 	C$tempo.c$43$1$95 ==.
                                   3525 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:43: relogio[HOR] = hora;
      0007A2 85 11 31         [24] 3526 	mov	(_relogio + 0x0003),_ini_relogio_PARM_4
                           0006FA  3527 	C$tempo.c$44$1$95 ==.
                                   3528 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:44: relogio[MIN] = minuto;
      0007A5 85 12 32         [24] 3529 	mov	(_relogio + 0x0004),_ini_relogio_PARM_5
                           0006FD  3530 	C$tempo.c$45$1$95 ==.
                                   3531 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:45: relogio[SEG] = segundo;
      0007A8 85 13 33         [24] 3532 	mov	(_relogio + 0x0005),_ini_relogio_PARM_6
                           000700  3533 	C$tempo.c$46$1$95 ==.
                           000700  3534 	XG$ini_relogio$0$0 ==.
      0007AB 22               [24] 3535 	ret
                                   3536 ;------------------------------------------------------------
                                   3537 ;Allocation info for local variables in function 'coleta_amostra'
                                   3538 ;------------------------------------------------------------
                                   3539 ;i                         Allocated to registers r7 
                                   3540 ;------------------------------------------------------------
                           000701  3541 	G$coleta_amostra$0$0 ==.
                           000701  3542 	C$tempo.c$48$1$95 ==.
                                   3543 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:48: void coleta_amostra(void){
                                   3544 ;	-----------------------------------------
                                   3545 ;	 function coleta_amostra
                                   3546 ;	-----------------------------------------
      0007AC                       3547 _coleta_amostra:
                           000701  3548 	C$tempo.c$53$1$97 ==.
                                   3549 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:53: if(saida[CHECK] == 1){
      0007AC 74 01            [12] 3550 	mov	a,#0x01
      0007AE B5 25 68         [24] 3551 	cjne	a,_saida,00113$
                           000706  3552 	C$tempo.c$54$1$97 ==.
                                   3553 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:54: for(i = 0; i < QT_TEMPO-1; i++){
      0007B1 7F 00            [12] 3554 	mov	r7,#0x00
      0007B3                       3555 00109$:
                           000708  3556 	C$tempo.c$55$3$99 ==.
                                   3557 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:55: WDTCN = 0xa5;
      0007B3 75 FF A5         [24] 3558 	mov	_WDTCN,#0xa5
                           00070B  3559 	C$tempo.c$56$3$99 ==.
                                   3560 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:56: esc_RAM_SPI(end_fim_ram, relogio[i]);
      0007B6 EF               [12] 3561 	mov	a,r7
      0007B7 24 2E            [12] 3562 	add	a,#_relogio
      0007B9 F9               [12] 3563 	mov	r1,a
      0007BA 87 0F            [24] 3564 	mov	_esc_RAM_SPI_PARM_2,@r1
      0007BC 85 2C 82         [24] 3565 	mov	dpl,_end_fim_ram
      0007BF 85 2D 83         [24] 3566 	mov	dph,(_end_fim_ram + 1)
      0007C2 C0 07            [24] 3567 	push	ar7
      0007C4 12 06 0C         [24] 3568 	lcall	_esc_RAM_SPI
      0007C7 D0 07            [24] 3569 	pop	ar7
                           00071E  3570 	C$tempo.c$57$3$99 ==.
                                   3571 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:57: end_fim_ram++;
      0007C9 74 01            [12] 3572 	mov	a,#0x01
      0007CB 25 2C            [12] 3573 	add	a,_end_fim_ram
      0007CD F5 2C            [12] 3574 	mov	_end_fim_ram,a
      0007CF E4               [12] 3575 	clr	a
      0007D0 35 2D            [12] 3576 	addc	a,(_end_fim_ram + 1)
      0007D2 F5 2D            [12] 3577 	mov	(_end_fim_ram + 1),a
                           000729  3578 	C$tempo.c$58$3$99 ==.
                                   3579 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:58: if(end_fim_ram >= 8192) end_fim_ram = 0;
      0007D4 74 E0            [12] 3580 	mov	a,#0x100 - 0x20
      0007D6 25 2D            [12] 3581 	add	a,(_end_fim_ram + 1)
      0007D8 50 05            [24] 3582 	jnc	00110$
      0007DA E4               [12] 3583 	clr	a
      0007DB F5 2C            [12] 3584 	mov	_end_fim_ram,a
      0007DD F5 2D            [12] 3585 	mov	(_end_fim_ram + 1),a
      0007DF                       3586 00110$:
                           000734  3587 	C$tempo.c$54$2$98 ==.
                                   3588 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:54: for(i = 0; i < QT_TEMPO-1; i++){
      0007DF 0F               [12] 3589 	inc	r7
      0007E0 BF 06 00         [24] 3590 	cjne	r7,#0x06,00138$
      0007E3                       3591 00138$:
      0007E3 40 CE            [24] 3592 	jc	00109$
                           00073A  3593 	C$tempo.c$60$1$97 ==.
                                   3594 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:60: for(i = 1; i < QT_VALORES; i++){
      0007E5 7F 01            [12] 3595 	mov	r7,#0x01
      0007E7                       3596 00111$:
                           00073C  3597 	C$tempo.c$61$3$100 ==.
                                   3598 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:61: WDTCN = 0xa5;
      0007E7 75 FF A5         [24] 3599 	mov	_WDTCN,#0xa5
                           00073F  3600 	C$tempo.c$62$3$100 ==.
                                   3601 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:62: esc_RAM_SPI(end_fim_ram, saida[i]);
      0007EA EF               [12] 3602 	mov	a,r7
      0007EB 24 25            [12] 3603 	add	a,#_saida
      0007ED F9               [12] 3604 	mov	r1,a
      0007EE 87 0F            [24] 3605 	mov	_esc_RAM_SPI_PARM_2,@r1
      0007F0 85 2C 82         [24] 3606 	mov	dpl,_end_fim_ram
      0007F3 85 2D 83         [24] 3607 	mov	dph,(_end_fim_ram + 1)
      0007F6 C0 07            [24] 3608 	push	ar7
      0007F8 12 06 0C         [24] 3609 	lcall	_esc_RAM_SPI
      0007FB D0 07            [24] 3610 	pop	ar7
                           000752  3611 	C$tempo.c$63$3$100 ==.
                                   3612 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:63: end_fim_ram++;
      0007FD 74 01            [12] 3613 	mov	a,#0x01
      0007FF 25 2C            [12] 3614 	add	a,_end_fim_ram
      000801 F5 2C            [12] 3615 	mov	_end_fim_ram,a
      000803 E4               [12] 3616 	clr	a
      000804 35 2D            [12] 3617 	addc	a,(_end_fim_ram + 1)
      000806 F5 2D            [12] 3618 	mov	(_end_fim_ram + 1),a
                           00075D  3619 	C$tempo.c$64$3$100 ==.
                                   3620 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:64: if(end_fim_ram >= 8192) end_fim_ram = 0;
      000808 74 E0            [12] 3621 	mov	a,#0x100 - 0x20
      00080A 25 2D            [12] 3622 	add	a,(_end_fim_ram + 1)
      00080C 50 05            [24] 3623 	jnc	00112$
      00080E E4               [12] 3624 	clr	a
      00080F F5 2C            [12] 3625 	mov	_end_fim_ram,a
      000811 F5 2D            [12] 3626 	mov	(_end_fim_ram + 1),a
      000813                       3627 00112$:
                           000768  3628 	C$tempo.c$60$2$98 ==.
                                   3629 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:60: for(i = 1; i < QT_VALORES; i++){
      000813 0F               [12] 3630 	inc	r7
      000814 BF 06 00         [24] 3631 	cjne	r7,#0x06,00141$
      000817                       3632 00141$:
      000817 40 CE            [24] 3633 	jc	00111$
      000819                       3634 00113$:
                           00076E  3635 	C$tempo.c$68$1$97 ==.
                           00076E  3636 	XG$coleta_amostra$0$0 ==.
      000819 22               [24] 3637 	ret
                                   3638 ;------------------------------------------------------------
                                   3639 ;Allocation info for local variables in function 'demonstra_amostras'
                                   3640 ;------------------------------------------------------------
                                   3641 ;i                         Allocated with name '_demonstra_amostras_i_1_102'
                                   3642 ;sloc0                     Allocated with name '_demonstra_amostras_sloc0_1_0'
                                   3643 ;sloc1                     Allocated with name '_demonstra_amostras_sloc1_1_0'
                                   3644 ;------------------------------------------------------------
                           00076F  3645 	G$demonstra_amostras$0$0 ==.
                           00076F  3646 	C$tempo.c$70$1$97 ==.
                                   3647 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:70: void demonstra_amostras(void){
                                   3648 ;	-----------------------------------------
                                   3649 ;	 function demonstra_amostras
                                   3650 ;	-----------------------------------------
      00081A                       3651 _demonstra_amostras:
                           00076F  3652 	C$tempo.c$74$1$102 ==.
                                   3653 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:74: printf_fast_f("\x09 \nImprimindo amostras no terminal.\nPressione qualquer tecla para sair.\n");
      00081A 74 EA            [12] 3654 	mov	a,#___str_4
      00081C C0 E0            [24] 3655 	push	acc
      00081E 74 17            [12] 3656 	mov	a,#(___str_4 >> 8)
      000820 C0 E0            [24] 3657 	push	acc
      000822 12 0E 0F         [24] 3658 	lcall	_printf_fast_f
      000825 15 81            [12] 3659 	dec	sp
      000827 15 81            [12] 3660 	dec	sp
                           00077E  3661 	C$tempo.c$75$2$103 ==.
                                   3662 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:75: for(i = 0; i < end_fim_ram; i+=QT_VALORES+QT_TEMPO-2){
      000829 E4               [12] 3663 	clr	a
      00082A F5 41            [12] 3664 	mov	_demonstra_amostras_i_1_102,a
      00082C F5 42            [12] 3665 	mov	(_demonstra_amostras_i_1_102 + 1),a
      00082E                       3666 00103$:
      00082E C3               [12] 3667 	clr	c
      00082F E5 41            [12] 3668 	mov	a,_demonstra_amostras_i_1_102
      000831 95 2C            [12] 3669 	subb	a,_end_fim_ram
      000833 E5 42            [12] 3670 	mov	a,(_demonstra_amostras_i_1_102 + 1)
      000835 95 2D            [12] 3671 	subb	a,(_end_fim_ram + 1)
      000837 40 03            [24] 3672 	jc	00114$
      000839 02 09 B4         [24] 3673 	ljmp	00105$
      00083C                       3674 00114$:
                           000791  3675 	C$tempo.c$76$2$103 ==.
                                   3676 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:76: printf_fast_f("%02d/%02d/2%03d | %02d:%02d:%02d |",	le_RAM_SPI(i)+1, le_RAM_SPI(i+1)+1, le_RAM_SPI(i+2), le_RAM_SPI(i+3), le_RAM_SPI(i+4), le_RAM_SPI(i+5));
      00083C 85 41 82         [24] 3677 	mov	dpl,_demonstra_amostras_i_1_102
      00083F 85 42 83         [24] 3678 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      000842 A3               [24] 3679 	inc	dptr
      000843 A3               [24] 3680 	inc	dptr
      000844 A3               [24] 3681 	inc	dptr
      000845 A3               [24] 3682 	inc	dptr
      000846 A3               [24] 3683 	inc	dptr
      000847 12 06 34         [24] 3684 	lcall	_le_RAM_SPI
      00084A AD 82            [24] 3685 	mov	r5,dpl
      00084C 7C 00            [12] 3686 	mov	r4,#0x00
      00084E 85 41 82         [24] 3687 	mov	dpl,_demonstra_amostras_i_1_102
      000851 85 42 83         [24] 3688 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      000854 A3               [24] 3689 	inc	dptr
      000855 A3               [24] 3690 	inc	dptr
      000856 A3               [24] 3691 	inc	dptr
      000857 A3               [24] 3692 	inc	dptr
      000858 C0 05            [24] 3693 	push	ar5
      00085A C0 04            [24] 3694 	push	ar4
      00085C 12 06 34         [24] 3695 	lcall	_le_RAM_SPI
      00085F AB 82            [24] 3696 	mov	r3,dpl
      000861 7A 00            [12] 3697 	mov	r2,#0x00
      000863 85 41 82         [24] 3698 	mov	dpl,_demonstra_amostras_i_1_102
      000866 85 42 83         [24] 3699 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      000869 A3               [24] 3700 	inc	dptr
      00086A A3               [24] 3701 	inc	dptr
      00086B A3               [24] 3702 	inc	dptr
      00086C C0 03            [24] 3703 	push	ar3
      00086E C0 02            [24] 3704 	push	ar2
      000870 12 06 34         [24] 3705 	lcall	_le_RAM_SPI
      000873 A8 82            [24] 3706 	mov	r0,dpl
      000875 79 00            [12] 3707 	mov	r1,#0x00
      000877 85 41 82         [24] 3708 	mov	dpl,_demonstra_amostras_i_1_102
      00087A 85 42 83         [24] 3709 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      00087D A3               [24] 3710 	inc	dptr
      00087E A3               [24] 3711 	inc	dptr
      00087F C0 01            [24] 3712 	push	ar1
      000881 C0 00            [24] 3713 	push	ar0
      000883 12 06 34         [24] 3714 	lcall	_le_RAM_SPI
      000886 AF 82            [24] 3715 	mov	r7,dpl
      000888 8F 43            [24] 3716 	mov	_demonstra_amostras_sloc0_1_0,r7
      00088A 75 44 00         [24] 3717 	mov	(_demonstra_amostras_sloc0_1_0 + 1),#0x00
      00088D 85 41 82         [24] 3718 	mov	dpl,_demonstra_amostras_i_1_102
      000890 85 42 83         [24] 3719 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      000893 A3               [24] 3720 	inc	dptr
      000894 12 06 34         [24] 3721 	lcall	_le_RAM_SPI
      000897 AF 82            [24] 3722 	mov	r7,dpl
      000899 7E 00            [12] 3723 	mov	r6,#0x00
      00089B 74 01            [12] 3724 	mov	a,#0x01
      00089D 2F               [12] 3725 	add	a,r7
      00089E F5 45            [12] 3726 	mov	_demonstra_amostras_sloc1_1_0,a
      0008A0 E4               [12] 3727 	clr	a
      0008A1 3E               [12] 3728 	addc	a,r6
      0008A2 F5 46            [12] 3729 	mov	(_demonstra_amostras_sloc1_1_0 + 1),a
      0008A4 85 41 82         [24] 3730 	mov	dpl,_demonstra_amostras_i_1_102
      0008A7 85 42 83         [24] 3731 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      0008AA 12 06 34         [24] 3732 	lcall	_le_RAM_SPI
      0008AD AF 82            [24] 3733 	mov	r7,dpl
      0008AF D0 00            [24] 3734 	pop	ar0
      0008B1 D0 01            [24] 3735 	pop	ar1
      0008B3 D0 02            [24] 3736 	pop	ar2
      0008B5 D0 03            [24] 3737 	pop	ar3
      0008B7 D0 04            [24] 3738 	pop	ar4
      0008B9 D0 05            [24] 3739 	pop	ar5
      0008BB 7E 00            [12] 3740 	mov	r6,#0x00
      0008BD 0F               [12] 3741 	inc	r7
      0008BE BF 00 01         [24] 3742 	cjne	r7,#0x00,00115$
      0008C1 0E               [12] 3743 	inc	r6
      0008C2                       3744 00115$:
      0008C2 C0 05            [24] 3745 	push	ar5
      0008C4 C0 04            [24] 3746 	push	ar4
      0008C6 C0 03            [24] 3747 	push	ar3
      0008C8 C0 02            [24] 3748 	push	ar2
      0008CA C0 00            [24] 3749 	push	ar0
      0008CC C0 01            [24] 3750 	push	ar1
      0008CE C0 43            [24] 3751 	push	_demonstra_amostras_sloc0_1_0
      0008D0 C0 44            [24] 3752 	push	(_demonstra_amostras_sloc0_1_0 + 1)
      0008D2 C0 45            [24] 3753 	push	_demonstra_amostras_sloc1_1_0
      0008D4 C0 46            [24] 3754 	push	(_demonstra_amostras_sloc1_1_0 + 1)
      0008D6 C0 07            [24] 3755 	push	ar7
      0008D8 C0 06            [24] 3756 	push	ar6
      0008DA 74 33            [12] 3757 	mov	a,#___str_5
      0008DC C0 E0            [24] 3758 	push	acc
      0008DE 74 18            [12] 3759 	mov	a,#(___str_5 >> 8)
      0008E0 C0 E0            [24] 3760 	push	acc
      0008E2 12 0E 0F         [24] 3761 	lcall	_printf_fast_f
      0008E5 E5 81            [12] 3762 	mov	a,sp
      0008E7 24 F2            [12] 3763 	add	a,#0xf2
      0008E9 F5 81            [12] 3764 	mov	sp,a
                           000840  3765 	C$tempo.c$77$2$103 ==.
                                   3766 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:77: printf_fast_f(" Umi = %2d %% | Temp = %2d �C | Luz = %3.02f V | Chuva = %u\n", le_RAM_SPI(i+6), le_RAM_SPI(i+7), le_voltagem((le_RAM_SPI(i+9)<<8)+le_RAM_SPI(i+8), GAIN_5), le_RAM_SPI(i+10));
      0008EB 74 0A            [12] 3767 	mov	a,#0x0a
      0008ED 25 41            [12] 3768 	add	a,_demonstra_amostras_i_1_102
      0008EF F5 82            [12] 3769 	mov	dpl,a
      0008F1 E4               [12] 3770 	clr	a
      0008F2 35 42            [12] 3771 	addc	a,(_demonstra_amostras_i_1_102 + 1)
      0008F4 F5 83            [12] 3772 	mov	dph,a
      0008F6 12 06 34         [24] 3773 	lcall	_le_RAM_SPI
      0008F9 AF 82            [24] 3774 	mov	r7,dpl
      0008FB 7E 00            [12] 3775 	mov	r6,#0x00
      0008FD 85 41 82         [24] 3776 	mov	dpl,_demonstra_amostras_i_1_102
      000900 85 42 83         [24] 3777 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      000903 A3               [24] 3778 	inc	dptr
      000904 A3               [24] 3779 	inc	dptr
      000905 A3               [24] 3780 	inc	dptr
      000906 A3               [24] 3781 	inc	dptr
      000907 A3               [24] 3782 	inc	dptr
      000908 A3               [24] 3783 	inc	dptr
      000909 A3               [24] 3784 	inc	dptr
      00090A A3               [24] 3785 	inc	dptr
      00090B A3               [24] 3786 	inc	dptr
      00090C C0 07            [24] 3787 	push	ar7
      00090E C0 06            [24] 3788 	push	ar6
      000910 12 06 34         [24] 3789 	lcall	_le_RAM_SPI
      000913 AC 82            [24] 3790 	mov	r4,dpl
      000915 7D 00            [12] 3791 	mov	r5,#0x00
      000917 85 41 82         [24] 3792 	mov	dpl,_demonstra_amostras_i_1_102
      00091A 85 42 83         [24] 3793 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      00091D A3               [24] 3794 	inc	dptr
      00091E A3               [24] 3795 	inc	dptr
      00091F A3               [24] 3796 	inc	dptr
      000920 A3               [24] 3797 	inc	dptr
      000921 A3               [24] 3798 	inc	dptr
      000922 A3               [24] 3799 	inc	dptr
      000923 A3               [24] 3800 	inc	dptr
      000924 A3               [24] 3801 	inc	dptr
      000925 C0 05            [24] 3802 	push	ar5
      000927 C0 04            [24] 3803 	push	ar4
      000929 12 06 34         [24] 3804 	lcall	_le_RAM_SPI
      00092C AB 82            [24] 3805 	mov	r3,dpl
      00092E D0 04            [24] 3806 	pop	ar4
      000930 D0 05            [24] 3807 	pop	ar5
      000932 7A 00            [12] 3808 	mov	r2,#0x00
      000934 EB               [12] 3809 	mov	a,r3
      000935 2D               [12] 3810 	add	a,r5
      000936 F5 82            [12] 3811 	mov	dpl,a
      000938 EA               [12] 3812 	mov	a,r2
      000939 3C               [12] 3813 	addc	a,r4
      00093A F5 83            [12] 3814 	mov	dph,a
      00093C 75 2B 06         [24] 3815 	mov	_le_voltagem_PARM_2,#0x06
      00093F 12 05 39         [24] 3816 	lcall	_le_voltagem
      000942 AA 82            [24] 3817 	mov	r2,dpl
      000944 AB 83            [24] 3818 	mov	r3,dph
      000946 AC F0            [24] 3819 	mov	r4,b
      000948 FD               [12] 3820 	mov	r5,a
      000949 85 41 82         [24] 3821 	mov	dpl,_demonstra_amostras_i_1_102
      00094C 85 42 83         [24] 3822 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      00094F A3               [24] 3823 	inc	dptr
      000950 A3               [24] 3824 	inc	dptr
      000951 A3               [24] 3825 	inc	dptr
      000952 A3               [24] 3826 	inc	dptr
      000953 A3               [24] 3827 	inc	dptr
      000954 A3               [24] 3828 	inc	dptr
      000955 A3               [24] 3829 	inc	dptr
      000956 C0 05            [24] 3830 	push	ar5
      000958 C0 04            [24] 3831 	push	ar4
      00095A C0 03            [24] 3832 	push	ar3
      00095C C0 02            [24] 3833 	push	ar2
      00095E 12 06 34         [24] 3834 	lcall	_le_RAM_SPI
      000961 A9 82            [24] 3835 	mov	r1,dpl
      000963 89 45            [24] 3836 	mov	_demonstra_amostras_sloc1_1_0,r1
      000965 75 46 00         [24] 3837 	mov	(_demonstra_amostras_sloc1_1_0 + 1),#0x00
      000968 85 41 82         [24] 3838 	mov	dpl,_demonstra_amostras_i_1_102
      00096B 85 42 83         [24] 3839 	mov	dph,(_demonstra_amostras_i_1_102 + 1)
      00096E A3               [24] 3840 	inc	dptr
      00096F A3               [24] 3841 	inc	dptr
      000970 A3               [24] 3842 	inc	dptr
      000971 A3               [24] 3843 	inc	dptr
      000972 A3               [24] 3844 	inc	dptr
      000973 A3               [24] 3845 	inc	dptr
      000974 12 06 34         [24] 3846 	lcall	_le_RAM_SPI
      000977 A9 82            [24] 3847 	mov	r1,dpl
      000979 D0 02            [24] 3848 	pop	ar2
      00097B D0 03            [24] 3849 	pop	ar3
      00097D D0 04            [24] 3850 	pop	ar4
      00097F D0 05            [24] 3851 	pop	ar5
      000981 89 00            [24] 3852 	mov	ar0,r1
      000983 79 00            [12] 3853 	mov	r1,#0x00
      000985 C0 02            [24] 3854 	push	ar2
      000987 C0 03            [24] 3855 	push	ar3
      000989 C0 04            [24] 3856 	push	ar4
      00098B C0 05            [24] 3857 	push	ar5
      00098D C0 45            [24] 3858 	push	_demonstra_amostras_sloc1_1_0
      00098F C0 46            [24] 3859 	push	(_demonstra_amostras_sloc1_1_0 + 1)
      000991 C0 00            [24] 3860 	push	ar0
      000993 C0 01            [24] 3861 	push	ar1
      000995 74 56            [12] 3862 	mov	a,#___str_6
      000997 C0 E0            [24] 3863 	push	acc
      000999 74 18            [12] 3864 	mov	a,#(___str_6 >> 8)
      00099B C0 E0            [24] 3865 	push	acc
      00099D 12 0E 0F         [24] 3866 	lcall	_printf_fast_f
      0009A0 E5 81            [12] 3867 	mov	a,sp
      0009A2 24 F4            [12] 3868 	add	a,#0xf4
      0009A4 F5 81            [12] 3869 	mov	sp,a
                           0008FB  3870 	C$tempo.c$75$1$102 ==.
                                   3871 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:75: for(i = 0; i < end_fim_ram; i+=QT_VALORES+QT_TEMPO-2){
      0009A6 74 0B            [12] 3872 	mov	a,#0x0b
      0009A8 25 41            [12] 3873 	add	a,_demonstra_amostras_i_1_102
      0009AA F5 41            [12] 3874 	mov	_demonstra_amostras_i_1_102,a
      0009AC E4               [12] 3875 	clr	a
      0009AD 35 42            [12] 3876 	addc	a,(_demonstra_amostras_i_1_102 + 1)
      0009AF F5 42            [12] 3877 	mov	(_demonstra_amostras_i_1_102 + 1),a
      0009B1 02 08 2E         [24] 3878 	ljmp	00103$
      0009B4                       3879 00105$:
                           000909  3880 	C$tempo.c$80$1$102 ==.
                           000909  3881 	XG$demonstra_amostras$0$0 ==.
      0009B4 22               [24] 3882 	ret
                                   3883 ;------------------------------------------------------------
                                   3884 ;Allocation info for local variables in function 'isr_tempo'
                                   3885 ;------------------------------------------------------------
                           00090A  3886 	G$isr_tempo$0$0 ==.
                           00090A  3887 	C$tempo.c$82$1$102 ==.
                                   3888 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:82: void isr_tempo(void) __interrupt 5{
                                   3889 ;	-----------------------------------------
                                   3890 ;	 function isr_tempo
                                   3891 ;	-----------------------------------------
      0009B5                       3892 _isr_tempo:
      0009B5 C0 23            [24] 3893 	push	bits
      0009B7 C0 E0            [24] 3894 	push	acc
      0009B9 C0 F0            [24] 3895 	push	b
      0009BB C0 82            [24] 3896 	push	dpl
      0009BD C0 83            [24] 3897 	push	dph
      0009BF C0 07            [24] 3898 	push	(0+7)
      0009C1 C0 06            [24] 3899 	push	(0+6)
      0009C3 C0 05            [24] 3900 	push	(0+5)
      0009C5 C0 04            [24] 3901 	push	(0+4)
      0009C7 C0 03            [24] 3902 	push	(0+3)
      0009C9 C0 02            [24] 3903 	push	(0+2)
      0009CB C0 01            [24] 3904 	push	(0+1)
      0009CD C0 00            [24] 3905 	push	(0+0)
      0009CF C0 D0            [24] 3906 	push	psw
      0009D1 75 D0 00         [24] 3907 	mov	psw,#0x00
                           000929  3908 	C$tempo.c$85$1$105 ==.
                                   3909 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:85: TF2 = 0;
      0009D4 C2 CF            [12] 3910 	clr	_TF2
                           00092B  3911 	C$tempo.c$87$1$105 ==.
                                   3912 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:87: if(relogio[MSE] == MSE_SEG) relogio[SEG]++, relogio[MSE]=0, le_sensores();
      0009D6 74 C7            [12] 3913 	mov	a,#0xc7
      0009D8 B5 34 0D         [24] 3914 	cjne	a,(_relogio + 0x0006),00102$
      0009DB E5 33            [12] 3915 	mov	a,(_relogio + 0x0005)
      0009DD 04               [12] 3916 	inc	a
      0009DE F5 33            [12] 3917 	mov	(_relogio + 0x0005),a
      0009E0 75 34 00         [24] 3918 	mov	(_relogio + 0x0006),#0x00
      0009E3 12 05 F2         [24] 3919 	lcall	_le_sensores
      0009E6 80 06            [24] 3920 	sjmp	00103$
      0009E8                       3921 00102$:
                           00093D  3922 	C$tempo.c$88$1$105 ==.
                                   3923 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:88: else relogio[MSE]++;
      0009E8 E5 34            [12] 3924 	mov	a,(_relogio + 0x0006)
      0009EA FF               [12] 3925 	mov	r7,a
      0009EB 04               [12] 3926 	inc	a
      0009EC F5 34            [12] 3927 	mov	(_relogio + 0x0006),a
      0009EE                       3928 00103$:
                           000943  3929 	C$tempo.c$90$1$105 ==.
                                   3930 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:90: if(relogio[SEG] >= SEG_MIN) relogio[MIN]++, relogio[SEG]=0, coleta_amostra();
      0009EE 74 C4            [12] 3931 	mov	a,#0x100 - 0x3c
      0009F0 25 33            [12] 3932 	add	a,(_relogio + 0x0005)
      0009F2 50 0B            [24] 3933 	jnc	00105$
      0009F4 E5 32            [12] 3934 	mov	a,(_relogio + 0x0004)
      0009F6 04               [12] 3935 	inc	a
      0009F7 F5 32            [12] 3936 	mov	(_relogio + 0x0004),a
      0009F9 75 33 00         [24] 3937 	mov	(_relogio + 0x0005),#0x00
      0009FC 12 07 AC         [24] 3938 	lcall	_coleta_amostra
      0009FF                       3939 00105$:
                           000954  3940 	C$tempo.c$91$1$105 ==.
                                   3941 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:91: if(relogio[MIN] >= SEG_MIN) relogio[HOR]++, relogio[MIN]=0;
      0009FF 74 C4            [12] 3942 	mov	a,#0x100 - 0x3c
      000A01 25 32            [12] 3943 	add	a,(_relogio + 0x0004)
      000A03 50 09            [24] 3944 	jnc	00107$
      000A05 E5 31            [12] 3945 	mov	a,(_relogio + 0x0003)
      000A07 FF               [12] 3946 	mov	r7,a
      000A08 04               [12] 3947 	inc	a
      000A09 F5 31            [12] 3948 	mov	(_relogio + 0x0003),a
      000A0B 75 32 00         [24] 3949 	mov	(_relogio + 0x0004),#0x00
      000A0E                       3950 00107$:
                           000963  3951 	C$tempo.c$92$1$105 ==.
                                   3952 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:92: if(relogio[HOR] >= HOR_DIA) relogio[DIA]++, relogio[HOR]=0;
      000A0E 74 E8            [12] 3953 	mov	a,#0x100 - 0x18
      000A10 25 31            [12] 3954 	add	a,(_relogio + 0x0003)
      000A12 50 09            [24] 3955 	jnc	00109$
      000A14 E5 2E            [12] 3956 	mov	a,_relogio
      000A16 FF               [12] 3957 	mov	r7,a
      000A17 04               [12] 3958 	inc	a
      000A18 F5 2E            [12] 3959 	mov	_relogio,a
      000A1A 75 31 00         [24] 3960 	mov	(_relogio + 0x0003),#0x00
      000A1D                       3961 00109$:
                           000972  3962 	C$tempo.c$93$1$105 ==.
                                   3963 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:93: if((relogio[MES]%2==0 && relogio[MES]<7 || relogio[MES]%2==1 && relogio[MES]>=7) && relogio[DIA]>29 || (relogio[MES]%2==1 && relogio[MES]<7 || relogio[MES]%2==0 && relogio[MES]>=7) && relogio[DIA]>28 || relogio[MES]==FEV && relogio[DIA]>(26+ano_bissexto())) relogio[MES]++, relogio[DIA]=0;
      000A1D E5 2F            [12] 3964 	mov	a,(_relogio + 0x0001)
      000A1F 20 E0 06         [24] 3965 	jb	acc.0,00114$
      000A22 74 F9            [12] 3966 	mov	a,#0x100 - 0x07
      000A24 25 2F            [12] 3967 	add	a,(_relogio + 0x0001)
      000A26 50 0E            [24] 3968 	jnc	00115$
      000A28                       3969 00114$:
      000A28 74 01            [12] 3970 	mov	a,#0x01
      000A2A 55 2F            [12] 3971 	anl	a,(_relogio + 0x0001)
      000A2C FF               [12] 3972 	mov	r7,a
      000A2D BF 01 0C         [24] 3973 	cjne	r7,#0x01,00120$
      000A30 74 F9            [12] 3974 	mov	a,#0x100 - 0x07
      000A32 25 2F            [12] 3975 	add	a,(_relogio + 0x0001)
      000A34 50 06            [24] 3976 	jnc	00120$
      000A36                       3977 00115$:
      000A36 E5 2E            [12] 3978 	mov	a,_relogio
      000A38 24 E2            [12] 3979 	add	a,#0xff - 0x1d
      000A3A 40 49            [24] 3980 	jc	00110$
      000A3C                       3981 00120$:
      000A3C 74 01            [12] 3982 	mov	a,#0x01
      000A3E 55 2F            [12] 3983 	anl	a,(_relogio + 0x0001)
      000A40 FF               [12] 3984 	mov	r7,a
      000A41 BF 01 06         [24] 3985 	cjne	r7,#0x01,00118$
      000A44 74 F9            [12] 3986 	mov	a,#0x100 - 0x07
      000A46 25 2F            [12] 3987 	add	a,(_relogio + 0x0001)
      000A48 50 0B            [24] 3988 	jnc	00119$
      000A4A                       3989 00118$:
      000A4A E5 2F            [12] 3990 	mov	a,(_relogio + 0x0001)
      000A4C 20 E0 0C         [24] 3991 	jb	acc.0,00122$
      000A4F 74 F9            [12] 3992 	mov	a,#0x100 - 0x07
      000A51 25 2F            [12] 3993 	add	a,(_relogio + 0x0001)
      000A53 50 06            [24] 3994 	jnc	00122$
      000A55                       3995 00119$:
      000A55 E5 2E            [12] 3996 	mov	a,_relogio
      000A57 24 E3            [12] 3997 	add	a,#0xff - 0x1c
      000A59 40 2A            [24] 3998 	jc	00110$
      000A5B                       3999 00122$:
      000A5B 74 01            [12] 4000 	mov	a,#0x01
      000A5D B5 2F 2E         [24] 4001 	cjne	a,(_relogio + 0x0001),00111$
      000A60 AF 2E            [24] 4002 	mov	r7,_relogio
      000A62 C0 07            [24] 4003 	push	ar7
      000A64 12 07 84         [24] 4004 	lcall	_ano_bissexto
      000A67 AE 82            [24] 4005 	mov	r6,dpl
      000A69 D0 07            [24] 4006 	pop	ar7
      000A6B 7D 00            [12] 4007 	mov	r5,#0x00
      000A6D 74 1A            [12] 4008 	mov	a,#0x1a
      000A6F 2E               [12] 4009 	add	a,r6
      000A70 FE               [12] 4010 	mov	r6,a
      000A71 E4               [12] 4011 	clr	a
      000A72 3D               [12] 4012 	addc	a,r5
      000A73 FD               [12] 4013 	mov	r5,a
      000A74 7C 00            [12] 4014 	mov	r4,#0x00
      000A76 C3               [12] 4015 	clr	c
      000A77 EE               [12] 4016 	mov	a,r6
      000A78 9F               [12] 4017 	subb	a,r7
      000A79 ED               [12] 4018 	mov	a,r5
      000A7A 64 80            [12] 4019 	xrl	a,#0x80
      000A7C 8C F0            [24] 4020 	mov	b,r4
      000A7E 63 F0 80         [24] 4021 	xrl	b,#0x80
      000A81 95 F0            [12] 4022 	subb	a,b
      000A83 50 09            [24] 4023 	jnc	00111$
      000A85                       4024 00110$:
      000A85 E5 2F            [12] 4025 	mov	a,(_relogio + 0x0001)
      000A87 FF               [12] 4026 	mov	r7,a
      000A88 04               [12] 4027 	inc	a
      000A89 F5 2F            [12] 4028 	mov	(_relogio + 0x0001),a
      000A8B 75 2E 00         [24] 4029 	mov	_relogio,#0x00
      000A8E                       4030 00111$:
                           0009E3  4031 	C$tempo.c$95$1$105 ==.
                                   4032 ;	C:\Users\202019050584\Desktop\Trabalho\/tempo.c:95: if(relogio[MES] == MES_ANO) relogio[ANO]++, relogio[MES]=0;
      000A8E 74 0C            [12] 4033 	mov	a,#0x0c
      000A90 B5 2F 09         [24] 4034 	cjne	a,(_relogio + 0x0001),00125$
      000A93 E5 30            [12] 4035 	mov	a,(_relogio + 0x0002)
      000A95 FF               [12] 4036 	mov	r7,a
      000A96 04               [12] 4037 	inc	a
      000A97 F5 30            [12] 4038 	mov	(_relogio + 0x0002),a
      000A99 75 2F 00         [24] 4039 	mov	(_relogio + 0x0001),#0x00
      000A9C                       4040 00125$:
      000A9C D0 D0            [24] 4041 	pop	psw
      000A9E D0 00            [24] 4042 	pop	(0+0)
      000AA0 D0 01            [24] 4043 	pop	(0+1)
      000AA2 D0 02            [24] 4044 	pop	(0+2)
      000AA4 D0 03            [24] 4045 	pop	(0+3)
      000AA6 D0 04            [24] 4046 	pop	(0+4)
      000AA8 D0 05            [24] 4047 	pop	(0+5)
      000AAA D0 06            [24] 4048 	pop	(0+6)
      000AAC D0 07            [24] 4049 	pop	(0+7)
      000AAE D0 83            [24] 4050 	pop	dph
      000AB0 D0 82            [24] 4051 	pop	dpl
      000AB2 D0 F0            [24] 4052 	pop	b
      000AB4 D0 E0            [24] 4053 	pop	acc
      000AB6 D0 23            [24] 4054 	pop	bits
                           000A0D  4055 	C$tempo.c$96$1$105 ==.
                           000A0D  4056 	XG$isr_tempo$0$0 ==.
      000AB8 32               [24] 4057 	reti
                                   4058 ;------------------------------------------------------------
                                   4059 ;Allocation info for local variables in function 'isr_UART0'
                                   4060 ;------------------------------------------------------------
                           000A0E  4061 	G$isr_UART0$0$0 ==.
                           000A0E  4062 	C$main.c$19$1$105 ==.
                                   4063 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:19: void isr_UART0(void) __interrupt 4{
                                   4064 ;	-----------------------------------------
                                   4065 ;	 function isr_UART0
                                   4066 ;	-----------------------------------------
      000AB9                       4067 _isr_UART0:
                           000A0E  4068 	C$main.c$21$1$107 ==.
                                   4069 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:21: if(RI0==1){
      000AB9 30 98 07         [24] 4070 	jnb	_RI0,00103$
                           000A11  4071 	C$main.c$22$2$108 ==.
                                   4072 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:22: tecla = SBUF0;
      000ABC 85 99 47         [24] 4073 	mov	_tecla,_SBUF0
                           000A14  4074 	C$main.c$23$2$108 ==.
                                   4075 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:23: flag_tecla = 1;
      000ABF D2 0C            [12] 4076 	setb	_flag_tecla
                           000A16  4077 	C$main.c$24$2$108 ==.
                                   4078 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:24: RI0 = 0;
      000AC1 C2 98            [12] 4079 	clr	_RI0
      000AC3                       4080 00103$:
                           000A18  4081 	C$main.c$26$1$107 ==.
                           000A18  4082 	XG$isr_UART0$0$0 ==.
      000AC3 32               [24] 4083 	reti
                                   4084 ;	eliminated unneeded mov psw,# (no regs used in bank)
                                   4085 ;	eliminated unneeded push/pop psw
                                   4086 ;	eliminated unneeded push/pop dpl
                                   4087 ;	eliminated unneeded push/pop dph
                                   4088 ;	eliminated unneeded push/pop b
                                   4089 ;	eliminated unneeded push/pop acc
                                   4090 ;------------------------------------------------------------
                                   4091 ;Allocation info for local variables in function 'ligar_buzzer'
                                   4092 ;------------------------------------------------------------
                                   4093 ;meio_periodo              Allocated with name '_ligar_buzzer_PARM_2'
                                   4094 ;ciclos                    Allocated to registers 
                                   4095 ;------------------------------------------------------------
                           000A19  4096 	G$ligar_buzzer$0$0 ==.
                           000A19  4097 	C$main.c$28$1$107 ==.
                                   4098 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:28: void ligar_buzzer(unsigned int ciclos, unsigned int meio_periodo){
                                   4099 ;	-----------------------------------------
                                   4100 ;	 function ligar_buzzer
                                   4101 ;	-----------------------------------------
      000AC4                       4102 _ligar_buzzer:
      000AC4 AE 82            [24] 4103 	mov	r6,dpl
      000AC6 AF 83            [24] 4104 	mov	r7,dph
                           000A1D  4105 	C$main.c$31$1$110 ==.
                                   4106 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:31: while(ciclos--){
      000AC8                       4107 00101$:
      000AC8 8E 04            [24] 4108 	mov	ar4,r6
      000ACA 8F 05            [24] 4109 	mov	ar5,r7
      000ACC 1E               [12] 4110 	dec	r6
      000ACD BE FF 01         [24] 4111 	cjne	r6,#0xff,00113$
      000AD0 1F               [12] 4112 	dec	r7
      000AD1                       4113 00113$:
      000AD1 EC               [12] 4114 	mov	a,r4
      000AD2 4D               [12] 4115 	orl	a,r5
      000AD3 60 20            [24] 4116 	jz	00104$
                           000A2A  4117 	C$main.c$32$2$111 ==.
                                   4118 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:32: P2_7 = 0;
      000AD5 C2 A7            [12] 4119 	clr	_P2_7
                           000A2C  4120 	C$main.c$33$2$111 ==.
                                   4121 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:33: delay_us(meio_periodo);
      000AD7 85 48 82         [24] 4122 	mov	dpl,_ligar_buzzer_PARM_2
      000ADA 85 49 83         [24] 4123 	mov	dph,(_ligar_buzzer_PARM_2 + 1)
      000ADD C0 07            [24] 4124 	push	ar7
      000ADF C0 06            [24] 4125 	push	ar6
      000AE1 12 04 27         [24] 4126 	lcall	_delay_us
                           000A39  4127 	C$main.c$34$2$111 ==.
                                   4128 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:34: P2_7 = 1;
      000AE4 D2 A7            [12] 4129 	setb	_P2_7
                           000A3B  4130 	C$main.c$35$2$111 ==.
                                   4131 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:35: delay_us(meio_periodo);
      000AE6 85 48 82         [24] 4132 	mov	dpl,_ligar_buzzer_PARM_2
      000AE9 85 49 83         [24] 4133 	mov	dph,(_ligar_buzzer_PARM_2 + 1)
      000AEC 12 04 27         [24] 4134 	lcall	_delay_us
      000AEF D0 06            [24] 4135 	pop	ar6
      000AF1 D0 07            [24] 4136 	pop	ar7
      000AF3 80 D3            [24] 4137 	sjmp	00101$
      000AF5                       4138 00104$:
                           000A4A  4139 	C$main.c$37$1$110 ==.
                           000A4A  4140 	XG$ligar_buzzer$0$0 ==.
      000AF5 22               [24] 4141 	ret
                                   4142 ;------------------------------------------------------------
                                   4143 ;Allocation info for local variables in function 'imprime_glcd_tempo_real'
                                   4144 ;------------------------------------------------------------
                                   4145 ;luz                       Allocated to registers r4 r5 r6 r7 
                                   4146 ;------------------------------------------------------------
                           000A4B  4147 	G$imprime_glcd_tempo_real$0$0 ==.
                           000A4B  4148 	C$main.c$39$1$110 ==.
                                   4149 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:39: void imprime_glcd_tempo_real(void){
                                   4150 ;	-----------------------------------------
                                   4151 ;	 function imprime_glcd_tempo_real
                                   4152 ;	-----------------------------------------
      000AF6                       4153 _imprime_glcd_tempo_real:
                           000A4B  4154 	C$main.c$42$1$113 ==.
                                   4155 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:42: printf_fast_f("\x09 \nImprimindo dados no GLCD.\nPressione qualquer tecla para sair.\n");
      000AF6 74 93            [12] 4156 	mov	a,#___str_7
      000AF8 C0 E0            [24] 4157 	push	acc
      000AFA 74 18            [12] 4158 	mov	a,#(___str_7 >> 8)
      000AFC C0 E0            [24] 4159 	push	acc
      000AFE 12 0E 0F         [24] 4160 	lcall	_printf_fast_f
      000B01 15 81            [12] 4161 	dec	sp
      000B03 15 81            [12] 4162 	dec	sp
                           000A5A  4163 	C$main.c$44$1$113 ==.
                                   4164 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:44: limpa_glcd(ESQ);
      000B05 C2 08            [12] 4165 	clr	_limpa_glcd_PARM_1
      000B07 12 02 91         [24] 4166 	lcall	_limpa_glcd
                           000A5F  4167 	C$main.c$45$1$113 ==.
                                   4168 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:45: limpa_glcd(DIR);
      000B0A D2 08            [12] 4169 	setb	_limpa_glcd_PARM_1
      000B0C 12 02 91         [24] 4170 	lcall	_limpa_glcd
                           000A64  4171 	C$main.c$46$3$115 ==.
                                   4172 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:46: do{
      000B0F                       4173 00115$:
                           000A64  4174 	C$main.c$47$2$114 ==.
                                   4175 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:47: WDTCN = 0xa5;
      000B0F 75 FF A5         [24] 4176 	mov	_WDTCN,#0xa5
                           000A67  4177 	C$main.c$49$2$114 ==.
                                   4178 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:49: if(saida[CHECK] == 1){
      000B12 74 01            [12] 4179 	mov	a,#0x01
      000B14 B5 25 02         [24] 4180 	cjne	a,_saida,00141$
      000B17 80 03            [24] 4181 	sjmp	00142$
      000B19                       4182 00141$:
      000B19 02 0C 68         [24] 4183 	ljmp	00114$
      000B1C                       4184 00142$:
                           000A71  4185 	C$main.c$50$3$115 ==.
                                   4186 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:50: luz = le_voltagem((saida[LDR_HI]<<8)+saida[LDR_LO], GAIN_5);
      000B1C AF 29            [24] 4187 	mov	r7,(_saida + 0x0004)
      000B1E 7E 00            [12] 4188 	mov	r6,#0x00
      000B20 AC 28            [24] 4189 	mov	r4,(_saida + 0x0003)
      000B22 7D 00            [12] 4190 	mov	r5,#0x00
      000B24 EC               [12] 4191 	mov	a,r4
      000B25 2E               [12] 4192 	add	a,r6
      000B26 F5 82            [12] 4193 	mov	dpl,a
      000B28 ED               [12] 4194 	mov	a,r5
      000B29 3F               [12] 4195 	addc	a,r7
      000B2A F5 83            [12] 4196 	mov	dph,a
      000B2C 75 2B 06         [24] 4197 	mov	_le_voltagem_PARM_2,#0x06
      000B2F 12 05 39         [24] 4198 	lcall	_le_voltagem
      000B32 AC 82            [24] 4199 	mov	r4,dpl
      000B34 AD 83            [24] 4200 	mov	r5,dph
      000B36 AE F0            [24] 4201 	mov	r6,b
      000B38 FF               [12] 4202 	mov	r7,a
                           000A8E  4203 	C$main.c$52$3$115 ==.
                                   4204 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:52: print_relogio_glcd();
      000B39 C0 07            [24] 4205 	push	ar7
      000B3B C0 06            [24] 4206 	push	ar6
      000B3D C0 05            [24] 4207 	push	ar5
      000B3F C0 04            [24] 4208 	push	ar4
      000B41 12 07 32         [24] 4209 	lcall	_print_relogio_glcd
                           000A99  4210 	C$main.c$53$3$115 ==.
                                   4211 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:53: printf_fast_f("\x03 UR = %2d %%", saida[I_RH]);
      000B44 AA 26            [24] 4212 	mov	r2,(_saida + 0x0001)
      000B46 7B 00            [12] 4213 	mov	r3,#0x00
      000B48 C0 02            [24] 4214 	push	ar2
      000B4A C0 03            [24] 4215 	push	ar3
      000B4C 74 D5            [12] 4216 	mov	a,#___str_8
      000B4E C0 E0            [24] 4217 	push	acc
      000B50 74 18            [12] 4218 	mov	a,#(___str_8 >> 8)
      000B52 C0 E0            [24] 4219 	push	acc
      000B54 12 0E 0F         [24] 4220 	lcall	_printf_fast_f
      000B57 E5 81            [12] 4221 	mov	a,sp
      000B59 24 FC            [12] 4222 	add	a,#0xfc
      000B5B F5 81            [12] 4223 	mov	sp,a
                           000AB2  4224 	C$main.c$54$3$115 ==.
                                   4225 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:54: printf_fast_f("\x04 Temp = %2d �C", saida[I_TEMP]);
      000B5D AA 27            [24] 4226 	mov	r2,(_saida + 0x0002)
      000B5F 7B 00            [12] 4227 	mov	r3,#0x00
      000B61 C0 02            [24] 4228 	push	ar2
      000B63 C0 03            [24] 4229 	push	ar3
      000B65 74 E3            [12] 4230 	mov	a,#___str_9
      000B67 C0 E0            [24] 4231 	push	acc
      000B69 74 18            [12] 4232 	mov	a,#(___str_9 >> 8)
      000B6B C0 E0            [24] 4233 	push	acc
      000B6D 12 0E 0F         [24] 4234 	lcall	_printf_fast_f
      000B70 E5 81            [12] 4235 	mov	a,sp
      000B72 24 FC            [12] 4236 	add	a,#0xfc
      000B74 F5 81            [12] 4237 	mov	sp,a
      000B76 D0 04            [24] 4238 	pop	ar4
      000B78 D0 05            [24] 4239 	pop	ar5
      000B7A D0 06            [24] 4240 	pop	ar6
      000B7C D0 07            [24] 4241 	pop	ar7
                           000AD3  4242 	C$main.c$56$1$113 ==.
                                   4243 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:56: if(luz > 3.0) printf_fast_f("\x05 Muito claro");
      000B7E C0 07            [24] 4244 	push	ar7
      000B80 C0 06            [24] 4245 	push	ar6
      000B82 C0 05            [24] 4246 	push	ar5
      000B84 C0 04            [24] 4247 	push	ar4
      000B86 E4               [12] 4248 	clr	a
      000B87 C0 E0            [24] 4249 	push	acc
      000B89 C0 E0            [24] 4250 	push	acc
      000B8B 74 40            [12] 4251 	mov	a,#0x40
      000B8D C0 E0            [24] 4252 	push	acc
      000B8F C0 E0            [24] 4253 	push	acc
      000B91 8C 82            [24] 4254 	mov	dpl,r4
      000B93 8D 83            [24] 4255 	mov	dph,r5
      000B95 8E F0            [24] 4256 	mov	b,r6
      000B97 EF               [12] 4257 	mov	a,r7
      000B98 12 13 D7         [24] 4258 	lcall	___fsgt
      000B9B AB 82            [24] 4259 	mov	r3,dpl
      000B9D E5 81            [12] 4260 	mov	a,sp
      000B9F 24 FC            [12] 4261 	add	a,#0xfc
      000BA1 F5 81            [12] 4262 	mov	sp,a
      000BA3 D0 04            [24] 4263 	pop	ar4
      000BA5 D0 05            [24] 4264 	pop	ar5
      000BA7 D0 06            [24] 4265 	pop	ar6
      000BA9 D0 07            [24] 4266 	pop	ar7
      000BAB EB               [12] 4267 	mov	a,r3
      000BAC 60 12            [24] 4268 	jz	00108$
      000BAE 74 F3            [12] 4269 	mov	a,#___str_10
      000BB0 C0 E0            [24] 4270 	push	acc
      000BB2 74 18            [12] 4271 	mov	a,#(___str_10 >> 8)
      000BB4 C0 E0            [24] 4272 	push	acc
      000BB6 12 0E 0F         [24] 4273 	lcall	_printf_fast_f
      000BB9 15 81            [12] 4274 	dec	sp
      000BBB 15 81            [12] 4275 	dec	sp
      000BBD 02 0C 43         [24] 4276 	ljmp	00109$
      000BC0                       4277 00108$:
                           000B15  4278 	C$main.c$57$1$113 ==.
                                   4279 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:57: else if(luz > 2.0) printf_fast_f("\x05 Claro");
      000BC0 C0 07            [24] 4280 	push	ar7
      000BC2 C0 06            [24] 4281 	push	ar6
      000BC4 C0 05            [24] 4282 	push	ar5
      000BC6 C0 04            [24] 4283 	push	ar4
      000BC8 E4               [12] 4284 	clr	a
      000BC9 C0 E0            [24] 4285 	push	acc
      000BCB C0 E0            [24] 4286 	push	acc
      000BCD C0 E0            [24] 4287 	push	acc
      000BCF 74 40            [12] 4288 	mov	a,#0x40
      000BD1 C0 E0            [24] 4289 	push	acc
      000BD3 8C 82            [24] 4290 	mov	dpl,r4
      000BD5 8D 83            [24] 4291 	mov	dph,r5
      000BD7 8E F0            [24] 4292 	mov	b,r6
      000BD9 EF               [12] 4293 	mov	a,r7
      000BDA 12 13 D7         [24] 4294 	lcall	___fsgt
      000BDD AB 82            [24] 4295 	mov	r3,dpl
      000BDF E5 81            [12] 4296 	mov	a,sp
      000BE1 24 FC            [12] 4297 	add	a,#0xfc
      000BE3 F5 81            [12] 4298 	mov	sp,a
      000BE5 D0 04            [24] 4299 	pop	ar4
      000BE7 D0 05            [24] 4300 	pop	ar5
      000BE9 D0 06            [24] 4301 	pop	ar6
      000BEB D0 07            [24] 4302 	pop	ar7
      000BED EB               [12] 4303 	mov	a,r3
      000BEE 60 11            [24] 4304 	jz	00105$
      000BF0 74 01            [12] 4305 	mov	a,#___str_11
      000BF2 C0 E0            [24] 4306 	push	acc
      000BF4 74 19            [12] 4307 	mov	a,#(___str_11 >> 8)
      000BF6 C0 E0            [24] 4308 	push	acc
      000BF8 12 0E 0F         [24] 4309 	lcall	_printf_fast_f
      000BFB 15 81            [12] 4310 	dec	sp
      000BFD 15 81            [12] 4311 	dec	sp
      000BFF 80 42            [24] 4312 	sjmp	00109$
      000C01                       4313 00105$:
                           000B56  4314 	C$main.c$58$1$113 ==.
                                   4315 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:58: else if(luz > 1.0) printf_fast_f("\x05 Escuro");
      000C01 E4               [12] 4316 	clr	a
      000C02 C0 E0            [24] 4317 	push	acc
      000C04 C0 E0            [24] 4318 	push	acc
      000C06 74 80            [12] 4319 	mov	a,#0x80
      000C08 C0 E0            [24] 4320 	push	acc
      000C0A 74 3F            [12] 4321 	mov	a,#0x3f
      000C0C C0 E0            [24] 4322 	push	acc
      000C0E 8C 82            [24] 4323 	mov	dpl,r4
      000C10 8D 83            [24] 4324 	mov	dph,r5
      000C12 8E F0            [24] 4325 	mov	b,r6
      000C14 EF               [12] 4326 	mov	a,r7
      000C15 12 13 D7         [24] 4327 	lcall	___fsgt
      000C18 AF 82            [24] 4328 	mov	r7,dpl
      000C1A E5 81            [12] 4329 	mov	a,sp
      000C1C 24 FC            [12] 4330 	add	a,#0xfc
      000C1E F5 81            [12] 4331 	mov	sp,a
      000C20 EF               [12] 4332 	mov	a,r7
      000C21 60 11            [24] 4333 	jz	00102$
      000C23 74 09            [12] 4334 	mov	a,#___str_12
      000C25 C0 E0            [24] 4335 	push	acc
      000C27 74 19            [12] 4336 	mov	a,#(___str_12 >> 8)
      000C29 C0 E0            [24] 4337 	push	acc
      000C2B 12 0E 0F         [24] 4338 	lcall	_printf_fast_f
      000C2E 15 81            [12] 4339 	dec	sp
      000C30 15 81            [12] 4340 	dec	sp
      000C32 80 0F            [24] 4341 	sjmp	00109$
      000C34                       4342 00102$:
                           000B89  4343 	C$main.c$59$3$115 ==.
                                   4344 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:59: else printf_fast_f("\x05 Muito escuro\n");
      000C34 74 12            [12] 4345 	mov	a,#___str_13
      000C36 C0 E0            [24] 4346 	push	acc
      000C38 74 19            [12] 4347 	mov	a,#(___str_13 >> 8)
      000C3A C0 E0            [24] 4348 	push	acc
      000C3C 12 0E 0F         [24] 4349 	lcall	_printf_fast_f
      000C3F 15 81            [12] 4350 	dec	sp
      000C41 15 81            [12] 4351 	dec	sp
      000C43                       4352 00109$:
                           000B98  4353 	C$main.c$61$3$115 ==.
                                   4354 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:61: if(saida[B_CHUVA] == 1)	printf_fast_f("\x06 Sem chuva");
      000C43 74 01            [12] 4355 	mov	a,#0x01
      000C45 B5 2A 11         [24] 4356 	cjne	a,(_saida + 0x0005),00111$
      000C48 74 22            [12] 4357 	mov	a,#___str_14
      000C4A C0 E0            [24] 4358 	push	acc
      000C4C 74 19            [12] 4359 	mov	a,#(___str_14 >> 8)
      000C4E C0 E0            [24] 4360 	push	acc
      000C50 12 0E 0F         [24] 4361 	lcall	_printf_fast_f
      000C53 15 81            [12] 4362 	dec	sp
      000C55 15 81            [12] 4363 	dec	sp
      000C57 80 0F            [24] 4364 	sjmp	00114$
      000C59                       4365 00111$:
                           000BAE  4366 	C$main.c$62$3$115 ==.
                                   4367 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:62: else printf_fast_f("\x06 Chovendo\n");
      000C59 74 2E            [12] 4368 	mov	a,#___str_15
      000C5B C0 E0            [24] 4369 	push	acc
      000C5D 74 19            [12] 4370 	mov	a,#(___str_15 >> 8)
      000C5F C0 E0            [24] 4371 	push	acc
      000C61 12 0E 0F         [24] 4372 	lcall	_printf_fast_f
      000C64 15 81            [12] 4373 	dec	sp
      000C66 15 81            [12] 4374 	dec	sp
      000C68                       4375 00114$:
                           000BBD  4376 	C$main.c$66$2$114 ==.
                                   4377 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:66: delay_ms(DELAY_LACO);
      000C68 90 01 F4         [24] 4378 	mov	dptr,#0x01f4
      000C6B 12 03 FF         [24] 4379 	lcall	_delay_ms
                           000BC3  4380 	C$main.c$67$2$114 ==.
                                   4381 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:67: limpa_glcd(ESQ);
      000C6E C2 08            [12] 4382 	clr	_limpa_glcd_PARM_1
      000C70 12 02 91         [24] 4383 	lcall	_limpa_glcd
                           000BC8  4384 	C$main.c$68$2$114 ==.
                                   4385 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:68: limpa_glcd(DIR);
      000C73 D2 08            [12] 4386 	setb	_limpa_glcd_PARM_1
      000C75 12 02 91         [24] 4387 	lcall	_limpa_glcd
      000C78 20 0C 03         [24] 4388 	jb	_flag_tecla,00148$
      000C7B 02 0B 0F         [24] 4389 	ljmp	00115$
      000C7E                       4390 00148$:
                           000BD3  4391 	C$main.c$70$1$113 ==.
                                   4392 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:70: printf_fast_f("\x09 \n");
      000C7E 74 3A            [12] 4393 	mov	a,#___str_16
      000C80 C0 E0            [24] 4394 	push	acc
      000C82 74 19            [12] 4395 	mov	a,#(___str_16 >> 8)
      000C84 C0 E0            [24] 4396 	push	acc
      000C86 12 0E 0F         [24] 4397 	lcall	_printf_fast_f
      000C89 15 81            [12] 4398 	dec	sp
      000C8B 15 81            [12] 4399 	dec	sp
                           000BE2  4400 	C$main.c$72$1$113 ==.
                                   4401 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:72: flag_tecla=0;
      000C8D C2 0C            [12] 4402 	clr	_flag_tecla
                           000BE4  4403 	C$main.c$73$1$113 ==.
                                   4404 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:73: ligar_buzzer(50,1500);
      000C8F 75 48 DC         [24] 4405 	mov	_ligar_buzzer_PARM_2,#0xdc
      000C92 75 49 05         [24] 4406 	mov	(_ligar_buzzer_PARM_2 + 1),#0x05
      000C95 90 00 32         [24] 4407 	mov	dptr,#0x0032
      000C98 12 0A C4         [24] 4408 	lcall	_ligar_buzzer
                           000BF0  4409 	C$main.c$74$1$113 ==.
                           000BF0  4410 	XG$imprime_glcd_tempo_real$0$0 ==.
      000C9B 22               [24] 4411 	ret
                                   4412 ;------------------------------------------------------------
                                   4413 ;Allocation info for local variables in function 'imprime_terminal_tempo_real'
                                   4414 ;------------------------------------------------------------
                                   4415 ;sloc0                     Allocated with name '_imprime_terminal_tempo_real_sloc0_1_0'
                                   4416 ;sloc1                     Allocated with name '_imprime_terminal_tempo_real_sloc1_1_0'
                                   4417 ;------------------------------------------------------------
                           000BF1  4418 	G$imprime_terminal_tempo_real$0$0 ==.
                           000BF1  4419 	C$main.c$76$1$113 ==.
                                   4420 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:76: void imprime_terminal_tempo_real(void){
                                   4421 ;	-----------------------------------------
                                   4422 ;	 function imprime_terminal_tempo_real
                                   4423 ;	-----------------------------------------
      000C9C                       4424 _imprime_terminal_tempo_real:
                           000BF1  4425 	C$main.c$77$1$117 ==.
                                   4426 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:77: printf_fast_f("\x09 \nImprimindo dados no terminal.\nPressione qualquer tecla para sair.\n");
      000C9C 74 3E            [12] 4427 	mov	a,#___str_17
      000C9E C0 E0            [24] 4428 	push	acc
      000CA0 74 19            [12] 4429 	mov	a,#(___str_17 >> 8)
      000CA2 C0 E0            [24] 4430 	push	acc
      000CA4 12 0E 0F         [24] 4431 	lcall	_printf_fast_f
      000CA7 15 81            [12] 4432 	dec	sp
      000CA9 15 81            [12] 4433 	dec	sp
                           000C00  4434 	C$main.c$79$3$119 ==.
                                   4435 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:79: do{
      000CAB                       4436 00103$:
                           000C00  4437 	C$main.c$80$2$118 ==.
                                   4438 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:80: WDTCN = 0xa5;
      000CAB 75 FF A5         [24] 4439 	mov	_WDTCN,#0xa5
                           000C03  4440 	C$main.c$82$2$118 ==.
                                   4441 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:82: if(saida[CHECK] == 1){
      000CAE 74 01            [12] 4442 	mov	a,#0x01
      000CB0 B5 25 58         [24] 4443 	cjne	a,_saida,00102$
                           000C08  4444 	C$main.c$83$3$119 ==.
                                   4445 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:83: print_relogio_terminal();
      000CB3 12 06 E0         [24] 4446 	lcall	_print_relogio_terminal
                           000C0B  4447 	C$main.c$84$3$119 ==.
                                   4448 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:84: printf_fast_f(" Umi = %2d %% | Temp = %2d �C | Luz = %3.02f V | Chuva = %u\r", saida[I_RH], saida[I_TEMP], le_voltagem((saida[LDR_HI]<<8)+saida[LDR_LO], GAIN_5), MHRD);
      000CB6 A2 86            [12] 4449 	mov	c,_P0_6
      000CB8 E4               [12] 4450 	clr	a
      000CB9 33               [12] 4451 	rlc	a
      000CBA F5 4A            [12] 4452 	mov	_imprime_terminal_tempo_real_sloc0_1_0,a
      000CBC 75 4B 00         [24] 4453 	mov	(_imprime_terminal_tempo_real_sloc0_1_0 + 1),#0x00
      000CBF AD 29            [24] 4454 	mov	r5,(_saida + 0x0004)
      000CC1 7C 00            [12] 4455 	mov	r4,#0x00
      000CC3 AA 28            [24] 4456 	mov	r2,(_saida + 0x0003)
      000CC5 7B 00            [12] 4457 	mov	r3,#0x00
      000CC7 EA               [12] 4458 	mov	a,r2
      000CC8 2C               [12] 4459 	add	a,r4
      000CC9 F5 82            [12] 4460 	mov	dpl,a
      000CCB EB               [12] 4461 	mov	a,r3
      000CCC 3D               [12] 4462 	addc	a,r5
      000CCD F5 83            [12] 4463 	mov	dph,a
      000CCF 75 2B 06         [24] 4464 	mov	_le_voltagem_PARM_2,#0x06
      000CD2 12 05 39         [24] 4465 	lcall	_le_voltagem
      000CD5 AA 82            [24] 4466 	mov	r2,dpl
      000CD7 AB 83            [24] 4467 	mov	r3,dph
      000CD9 AC F0            [24] 4468 	mov	r4,b
      000CDB FD               [12] 4469 	mov	r5,a
      000CDC 85 27 4C         [24] 4470 	mov	_imprime_terminal_tempo_real_sloc1_1_0,(_saida + 0x0002)
      000CDF 75 4D 00         [24] 4471 	mov	(_imprime_terminal_tempo_real_sloc1_1_0 + 1),#0x00
      000CE2 AE 26            [24] 4472 	mov	r6,(_saida + 0x0001)
      000CE4 7F 00            [12] 4473 	mov	r7,#0x00
      000CE6 C0 4A            [24] 4474 	push	_imprime_terminal_tempo_real_sloc0_1_0
      000CE8 C0 4B            [24] 4475 	push	(_imprime_terminal_tempo_real_sloc0_1_0 + 1)
      000CEA C0 02            [24] 4476 	push	ar2
      000CEC C0 03            [24] 4477 	push	ar3
      000CEE C0 04            [24] 4478 	push	ar4
      000CF0 C0 05            [24] 4479 	push	ar5
      000CF2 C0 4C            [24] 4480 	push	_imprime_terminal_tempo_real_sloc1_1_0
      000CF4 C0 4D            [24] 4481 	push	(_imprime_terminal_tempo_real_sloc1_1_0 + 1)
      000CF6 C0 06            [24] 4482 	push	ar6
      000CF8 C0 07            [24] 4483 	push	ar7
      000CFA 74 84            [12] 4484 	mov	a,#___str_18
      000CFC C0 E0            [24] 4485 	push	acc
      000CFE 74 19            [12] 4486 	mov	a,#(___str_18 >> 8)
      000D00 C0 E0            [24] 4487 	push	acc
      000D02 12 0E 0F         [24] 4488 	lcall	_printf_fast_f
      000D05 E5 81            [12] 4489 	mov	a,sp
      000D07 24 F4            [12] 4490 	add	a,#0xf4
      000D09 F5 81            [12] 4491 	mov	sp,a
      000D0B                       4492 00102$:
                           000C60  4493 	C$main.c$87$2$118 ==.
                                   4494 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:87: delay_ms(DELAY_LACO);
      000D0B 90 01 F4         [24] 4495 	mov	dptr,#0x01f4
      000D0E 12 03 FF         [24] 4496 	lcall	_delay_ms
      000D11 30 0C 97         [24] 4497 	jnb	_flag_tecla,00103$
                           000C69  4498 	C$main.c$89$1$117 ==.
                                   4499 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:89: printf_fast_f("\x09 \n");
      000D14 74 3A            [12] 4500 	mov	a,#___str_16
      000D16 C0 E0            [24] 4501 	push	acc
      000D18 74 19            [12] 4502 	mov	a,#(___str_16 >> 8)
      000D1A C0 E0            [24] 4503 	push	acc
      000D1C 12 0E 0F         [24] 4504 	lcall	_printf_fast_f
      000D1F 15 81            [12] 4505 	dec	sp
      000D21 15 81            [12] 4506 	dec	sp
                           000C78  4507 	C$main.c$91$1$117 ==.
                                   4508 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:91: flag_tecla=0;
      000D23 C2 0C            [12] 4509 	clr	_flag_tecla
                           000C7A  4510 	C$main.c$92$1$117 ==.
                                   4511 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:92: ligar_buzzer(50,1500);
      000D25 75 48 DC         [24] 4512 	mov	_ligar_buzzer_PARM_2,#0xdc
      000D28 75 49 05         [24] 4513 	mov	(_ligar_buzzer_PARM_2 + 1),#0x05
      000D2B 90 00 32         [24] 4514 	mov	dptr,#0x0032
      000D2E 12 0A C4         [24] 4515 	lcall	_ligar_buzzer
                           000C86  4516 	C$main.c$93$1$117 ==.
                           000C86  4517 	XG$imprime_terminal_tempo_real$0$0 ==.
      000D31 22               [24] 4518 	ret
                                   4519 ;------------------------------------------------------------
                                   4520 ;Allocation info for local variables in function 'executa_comando'
                                   4521 ;------------------------------------------------------------
                           000C87  4522 	G$executa_comando$0$0 ==.
                           000C87  4523 	C$main.c$97$1$117 ==.
                                   4524 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:97: void executa_comando(void){
                                   4525 ;	-----------------------------------------
                                   4526 ;	 function executa_comando
                                   4527 ;	-----------------------------------------
      000D32                       4528 _executa_comando:
                           000C87  4529 	C$main.c$99$1$121 ==.
                                   4530 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:99: WDTCN = 0xa5;
      000D32 75 FF A5         [24] 4531 	mov	_WDTCN,#0xa5
                           000C8A  4532 	C$main.c$101$1$121 ==.
                                   4533 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:101: if(tecla == 'a') ligar_buzzer(50,800), imprime_terminal_tempo_real();
      000D35 74 61            [12] 4534 	mov	a,#0x61
      000D37 B5 47 12         [24] 4535 	cjne	a,_tecla,00111$
      000D3A 75 48 20         [24] 4536 	mov	_ligar_buzzer_PARM_2,#0x20
      000D3D 75 49 03         [24] 4537 	mov	(_ligar_buzzer_PARM_2 + 1),#0x03
      000D40 90 00 32         [24] 4538 	mov	dptr,#0x0032
      000D43 12 0A C4         [24] 4539 	lcall	_ligar_buzzer
      000D46 12 0C 9C         [24] 4540 	lcall	_imprime_terminal_tempo_real
      000D49 02 0D B5         [24] 4541 	ljmp	00113$
      000D4C                       4542 00111$:
                           000CA1  4543 	C$main.c$102$1$121 ==.
                                   4544 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:102: else if(tecla == 'b') ligar_buzzer(50,600), imprime_glcd_tempo_real();
      000D4C 74 62            [12] 4545 	mov	a,#0x62
      000D4E B5 47 11         [24] 4546 	cjne	a,_tecla,00108$
      000D51 75 48 58         [24] 4547 	mov	_ligar_buzzer_PARM_2,#0x58
      000D54 75 49 02         [24] 4548 	mov	(_ligar_buzzer_PARM_2 + 1),#0x02
      000D57 90 00 32         [24] 4549 	mov	dptr,#0x0032
      000D5A 12 0A C4         [24] 4550 	lcall	_ligar_buzzer
      000D5D 12 0A F6         [24] 4551 	lcall	_imprime_glcd_tempo_real
      000D60 80 53            [24] 4552 	sjmp	00113$
      000D62                       4553 00108$:
                           000CB7  4554 	C$main.c$103$1$121 ==.
                                   4555 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:103: else if(tecla == 'd') ligar_buzzer(50,400), demonstra_amostras();
      000D62 74 64            [12] 4556 	mov	a,#0x64
      000D64 B5 47 11         [24] 4557 	cjne	a,_tecla,00105$
      000D67 75 48 90         [24] 4558 	mov	_ligar_buzzer_PARM_2,#0x90
      000D6A 75 49 01         [24] 4559 	mov	(_ligar_buzzer_PARM_2 + 1),#0x01
      000D6D 90 00 32         [24] 4560 	mov	dptr,#0x0032
      000D70 12 0A C4         [24] 4561 	lcall	_ligar_buzzer
      000D73 12 08 1A         [24] 4562 	lcall	_demonstra_amostras
      000D76 80 3D            [24] 4563 	sjmp	00113$
      000D78                       4564 00105$:
                           000CCD  4565 	C$main.c$104$1$121 ==.
                                   4566 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:104: else if(tecla == 'm') ligar_buzzer(50,200), printf_fast_f("\x09 \nMENU:\na - Leitura no terminal\nb - Leitura no GLCD\nd - Imprime amostras coletadas\n");
      000D78 74 6D            [12] 4567 	mov	a,#0x6d
      000D7A B5 47 1D         [24] 4568 	cjne	a,_tecla,00102$
      000D7D 75 48 C8         [24] 4569 	mov	_ligar_buzzer_PARM_2,#0xc8
      000D80 75 49 00         [24] 4570 	mov	(_ligar_buzzer_PARM_2 + 1),#0x00
      000D83 90 00 32         [24] 4571 	mov	dptr,#0x0032
      000D86 12 0A C4         [24] 4572 	lcall	_ligar_buzzer
      000D89 74 C1            [12] 4573 	mov	a,#___str_19
      000D8B C0 E0            [24] 4574 	push	acc
      000D8D 74 19            [12] 4575 	mov	a,#(___str_19 >> 8)
      000D8F C0 E0            [24] 4576 	push	acc
      000D91 12 0E 0F         [24] 4577 	lcall	_printf_fast_f
      000D94 15 81            [12] 4578 	dec	sp
      000D96 15 81            [12] 4579 	dec	sp
      000D98 80 1B            [24] 4580 	sjmp	00113$
      000D9A                       4581 00102$:
                           000CEF  4582 	C$main.c$105$1$121 ==.
                                   4583 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:105: else ligar_buzzer(50,2000), printf_fast_f("\x09 \nDEFAULT\n");
      000D9A 75 48 D0         [24] 4584 	mov	_ligar_buzzer_PARM_2,#0xd0
      000D9D 75 49 07         [24] 4585 	mov	(_ligar_buzzer_PARM_2 + 1),#0x07
      000DA0 90 00 32         [24] 4586 	mov	dptr,#0x0032
      000DA3 12 0A C4         [24] 4587 	lcall	_ligar_buzzer
      000DA6 74 16            [12] 4588 	mov	a,#___str_20
      000DA8 C0 E0            [24] 4589 	push	acc
      000DAA 74 1A            [12] 4590 	mov	a,#(___str_20 >> 8)
      000DAC C0 E0            [24] 4591 	push	acc
      000DAE 12 0E 0F         [24] 4592 	lcall	_printf_fast_f
      000DB1 15 81            [12] 4593 	dec	sp
      000DB3 15 81            [12] 4594 	dec	sp
      000DB5                       4595 00113$:
                           000D0A  4596 	C$main.c$106$1$121 ==.
                           000D0A  4597 	XG$executa_comando$0$0 ==.
      000DB5 22               [24] 4598 	ret
                                   4599 ;------------------------------------------------------------
                                   4600 ;Allocation info for local variables in function 'main'
                                   4601 ;------------------------------------------------------------
                           000D0B  4602 	G$main$0$0 ==.
                           000D0B  4603 	C$main.c$108$1$121 ==.
                                   4604 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:108: void main(void){
                                   4605 ;	-----------------------------------------
                                   4606 ;	 function main
                                   4607 ;	-----------------------------------------
      000DB6                       4608 _main:
                           000D0B  4609 	C$main.c$109$1$123 ==.
                                   4610 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:109: Init_Device();
      000DB6 12 01 50         [24] 4611 	lcall	_Init_Device
                           000D0E  4612 	C$main.c$110$1$123 ==.
                                   4613 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:110: SFRPAGE=LEGACY_PAGE;
      000DB9 75 84 00         [24] 4614 	mov	_SFRPAGE,#0x00
                           000D11  4615 	C$main.c$112$1$123 ==.
                                   4616 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:112: ini_glcd();
      000DBC 12 02 02         [24] 4617 	lcall	_ini_glcd
                           000D14  4618 	C$main.c$113$1$123 ==.
                                   4619 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:113: limpa_glcd(ESQ);
      000DBF C2 08            [12] 4620 	clr	_limpa_glcd_PARM_1
      000DC1 12 02 91         [24] 4621 	lcall	_limpa_glcd
                           000D19  4622 	C$main.c$114$1$123 ==.
                                   4623 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:114: limpa_glcd(DIR);
      000DC4 D2 08            [12] 4624 	setb	_limpa_glcd_PARM_1
      000DC6 12 02 91         [24] 4625 	lcall	_limpa_glcd
                           000D1E  4626 	C$main.c$116$1$123 ==.
                                   4627 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:116: MHRD = 1;
      000DC9 D2 86            [12] 4628 	setb	_P0_6
                           000D20  4629 	C$main.c$117$1$123 ==.
                                   4630 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:117: ini_relogio(22, 06, 23, 13, 50, 00);
      000DCB 75 0F 06         [24] 4631 	mov	_ini_relogio_PARM_2,#0x06
      000DCE 75 10 17         [24] 4632 	mov	_ini_relogio_PARM_3,#0x17
      000DD1 75 11 0D         [24] 4633 	mov	_ini_relogio_PARM_4,#0x0d
      000DD4 75 12 32         [24] 4634 	mov	_ini_relogio_PARM_5,#0x32
      000DD7 75 13 00         [24] 4635 	mov	_ini_relogio_PARM_6,#0x00
      000DDA 75 82 16         [24] 4636 	mov	dpl,#0x16
      000DDD 12 07 95         [24] 4637 	lcall	_ini_relogio
                           000D35  4638 	C$main.c$119$1$123 ==.
                                   4639 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:119: ligar_buzzer(100, 1000);
      000DE0 75 48 E8         [24] 4640 	mov	_ligar_buzzer_PARM_2,#0xe8
      000DE3 75 49 03         [24] 4641 	mov	(_ligar_buzzer_PARM_2 + 1),#0x03
      000DE6 90 00 64         [24] 4642 	mov	dptr,#0x0064
      000DE9 12 0A C4         [24] 4643 	lcall	_ligar_buzzer
                           000D41  4644 	C$main.c$121$1$123 ==.
                                   4645 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:121: printf_fast_f("\x09 \nSTART\n");
      000DEC 74 22            [12] 4646 	mov	a,#___str_21
      000DEE C0 E0            [24] 4647 	push	acc
      000DF0 74 1A            [12] 4648 	mov	a,#(___str_21 >> 8)
      000DF2 C0 E0            [24] 4649 	push	acc
      000DF4 12 0E 0F         [24] 4650 	lcall	_printf_fast_f
      000DF7 15 81            [12] 4651 	dec	sp
      000DF9 15 81            [12] 4652 	dec	sp
                           000D50  4653 	C$main.c$122$1$123 ==.
                                   4654 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:122: while(1){
      000DFB                       4655 00104$:
                           000D50  4656 	C$main.c$123$2$124 ==.
                                   4657 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:123: WDTCN = 0xa5;
      000DFB 75 FF A5         [24] 4658 	mov	_WDTCN,#0xa5
                           000D53  4659 	C$main.c$125$2$124 ==.
                                   4660 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:125: if(flag_tecla==1){
                           000D53  4661 	C$main.c$126$3$125 ==.
                                   4662 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:126: flag_tecla = 0;
      000DFE 10 0C 02         [24] 4663 	jbc	_flag_tecla,00114$
      000E01 80 03            [24] 4664 	sjmp	00102$
      000E03                       4665 00114$:
                           000D58  4666 	C$main.c$127$3$125 ==.
                                   4667 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:127: executa_comando();
      000E03 12 0D 32         [24] 4668 	lcall	_executa_comando
      000E06                       4669 00102$:
                           000D5B  4670 	C$main.c$130$2$124 ==.
                                   4671 ;	C:\Users\202019050584\Desktop\Trabalho\main.c:130: delay_ms(DELAY_LACO);		
      000E06 90 01 F4         [24] 4672 	mov	dptr,#0x01f4
      000E09 12 03 FF         [24] 4673 	lcall	_delay_ms
      000E0C 80 ED            [24] 4674 	sjmp	00104$
                           000D63  4675 	C$main.c$132$1$123 ==.
                           000D63  4676 	XG$main$0$0 ==.
      000E0E 22               [24] 4677 	ret
                                   4678 	.area CSEG    (CODE)
                                   4679 	.area CONST   (CODE)
                           000000  4680 G$fonte$0$0 == .
      0015A1                       4681 _fonte:
      0015A1 00                    4682 	.db #0x00	; 0
      0015A2 00                    4683 	.db #0x00	; 0
      0015A3 00                    4684 	.db #0x00	; 0
      0015A4 00                    4685 	.db #0x00	; 0
      0015A5 00                    4686 	.db #0x00	; 0
      0015A6 00                    4687 	.db #0x00	; 0
      0015A7 00                    4688 	.db #0x00	; 0
      0015A8 5F                    4689 	.db #0x5f	; 95
      0015A9 00                    4690 	.db #0x00	; 0
      0015AA 00                    4691 	.db #0x00	; 0
      0015AB 00                    4692 	.db #0x00	; 0
      0015AC 07                    4693 	.db #0x07	; 7
      0015AD 00                    4694 	.db #0x00	; 0
      0015AE 07                    4695 	.db #0x07	; 7
      0015AF 00                    4696 	.db #0x00	; 0
      0015B0 14                    4697 	.db #0x14	; 20
      0015B1 7F                    4698 	.db #0x7f	; 127
      0015B2 14                    4699 	.db #0x14	; 20
      0015B3 7F                    4700 	.db #0x7f	; 127
      0015B4 14                    4701 	.db #0x14	; 20
      0015B5 24                    4702 	.db #0x24	; 36
      0015B6 2A                    4703 	.db #0x2a	; 42
      0015B7 7F                    4704 	.db #0x7f	; 127
      0015B8 2A                    4705 	.db #0x2a	; 42
      0015B9 12                    4706 	.db #0x12	; 18
      0015BA 23                    4707 	.db #0x23	; 35
      0015BB 13                    4708 	.db #0x13	; 19
      0015BC 08                    4709 	.db #0x08	; 8
      0015BD 64                    4710 	.db #0x64	; 100	'd'
      0015BE 62                    4711 	.db #0x62	; 98	'b'
      0015BF 36                    4712 	.db #0x36	; 54	'6'
      0015C0 49                    4713 	.db #0x49	; 73	'I'
      0015C1 55                    4714 	.db #0x55	; 85	'U'
      0015C2 22                    4715 	.db #0x22	; 34
      0015C3 50                    4716 	.db #0x50	; 80	'P'
      0015C4 00                    4717 	.db #0x00	; 0
      0015C5 05                    4718 	.db #0x05	; 5
      0015C6 03                    4719 	.db #0x03	; 3
      0015C7 00                    4720 	.db #0x00	; 0
      0015C8 00                    4721 	.db #0x00	; 0
      0015C9 00                    4722 	.db #0x00	; 0
      0015CA 1C                    4723 	.db #0x1c	; 28
      0015CB 22                    4724 	.db #0x22	; 34
      0015CC 41                    4725 	.db #0x41	; 65	'A'
      0015CD 00                    4726 	.db #0x00	; 0
      0015CE 00                    4727 	.db #0x00	; 0
      0015CF 41                    4728 	.db #0x41	; 65	'A'
      0015D0 22                    4729 	.db #0x22	; 34
      0015D1 1C                    4730 	.db #0x1c	; 28
      0015D2 00                    4731 	.db #0x00	; 0
      0015D3 08                    4732 	.db #0x08	; 8
      0015D4 2A                    4733 	.db #0x2a	; 42
      0015D5 1C                    4734 	.db #0x1c	; 28
      0015D6 2A                    4735 	.db #0x2a	; 42
      0015D7 08                    4736 	.db #0x08	; 8
      0015D8 08                    4737 	.db #0x08	; 8
      0015D9 08                    4738 	.db #0x08	; 8
      0015DA 3E                    4739 	.db #0x3e	; 62
      0015DB 08                    4740 	.db #0x08	; 8
      0015DC 08                    4741 	.db #0x08	; 8
      0015DD 00                    4742 	.db #0x00	; 0
      0015DE 50                    4743 	.db #0x50	; 80	'P'
      0015DF 30                    4744 	.db #0x30	; 48	'0'
      0015E0 00                    4745 	.db #0x00	; 0
      0015E1 00                    4746 	.db #0x00	; 0
      0015E2 08                    4747 	.db #0x08	; 8
      0015E3 08                    4748 	.db #0x08	; 8
      0015E4 08                    4749 	.db #0x08	; 8
      0015E5 08                    4750 	.db #0x08	; 8
      0015E6 08                    4751 	.db #0x08	; 8
      0015E7 00                    4752 	.db #0x00	; 0
      0015E8 30                    4753 	.db #0x30	; 48	'0'
      0015E9 30                    4754 	.db #0x30	; 48	'0'
      0015EA 00                    4755 	.db #0x00	; 0
      0015EB 00                    4756 	.db #0x00	; 0
      0015EC 20                    4757 	.db #0x20	; 32
      0015ED 10                    4758 	.db #0x10	; 16
      0015EE 08                    4759 	.db #0x08	; 8
      0015EF 04                    4760 	.db #0x04	; 4
      0015F0 02                    4761 	.db #0x02	; 2
      0015F1 3E                    4762 	.db #0x3e	; 62
      0015F2 51                    4763 	.db #0x51	; 81	'Q'
      0015F3 49                    4764 	.db #0x49	; 73	'I'
      0015F4 45                    4765 	.db #0x45	; 69	'E'
      0015F5 3E                    4766 	.db #0x3e	; 62
      0015F6 00                    4767 	.db #0x00	; 0
      0015F7 42                    4768 	.db #0x42	; 66	'B'
      0015F8 7F                    4769 	.db #0x7f	; 127
      0015F9 40                    4770 	.db #0x40	; 64
      0015FA 00                    4771 	.db #0x00	; 0
      0015FB 42                    4772 	.db #0x42	; 66	'B'
      0015FC 61                    4773 	.db #0x61	; 97	'a'
      0015FD 51                    4774 	.db #0x51	; 81	'Q'
      0015FE 49                    4775 	.db #0x49	; 73	'I'
      0015FF 46                    4776 	.db #0x46	; 70	'F'
      001600 21                    4777 	.db #0x21	; 33
      001601 41                    4778 	.db #0x41	; 65	'A'
      001602 45                    4779 	.db #0x45	; 69	'E'
      001603 4B                    4780 	.db #0x4b	; 75	'K'
      001604 31                    4781 	.db #0x31	; 49	'1'
      001605 18                    4782 	.db #0x18	; 24
      001606 14                    4783 	.db #0x14	; 20
      001607 12                    4784 	.db #0x12	; 18
      001608 7F                    4785 	.db #0x7f	; 127
      001609 10                    4786 	.db #0x10	; 16
      00160A 27                    4787 	.db #0x27	; 39
      00160B 45                    4788 	.db #0x45	; 69	'E'
      00160C 45                    4789 	.db #0x45	; 69	'E'
      00160D 45                    4790 	.db #0x45	; 69	'E'
      00160E 39                    4791 	.db #0x39	; 57	'9'
      00160F 3C                    4792 	.db #0x3c	; 60
      001610 4A                    4793 	.db #0x4a	; 74	'J'
      001611 49                    4794 	.db #0x49	; 73	'I'
      001612 49                    4795 	.db #0x49	; 73	'I'
      001613 30                    4796 	.db #0x30	; 48	'0'
      001614 01                    4797 	.db #0x01	; 1
      001615 71                    4798 	.db #0x71	; 113	'q'
      001616 09                    4799 	.db #0x09	; 9
      001617 05                    4800 	.db #0x05	; 5
      001618 03                    4801 	.db #0x03	; 3
      001619 36                    4802 	.db #0x36	; 54	'6'
      00161A 49                    4803 	.db #0x49	; 73	'I'
      00161B 49                    4804 	.db #0x49	; 73	'I'
      00161C 49                    4805 	.db #0x49	; 73	'I'
      00161D 36                    4806 	.db #0x36	; 54	'6'
      00161E 06                    4807 	.db #0x06	; 6
      00161F 49                    4808 	.db #0x49	; 73	'I'
      001620 49                    4809 	.db #0x49	; 73	'I'
      001621 29                    4810 	.db #0x29	; 41
      001622 1E                    4811 	.db #0x1e	; 30
      001623 00                    4812 	.db #0x00	; 0
      001624 36                    4813 	.db #0x36	; 54	'6'
      001625 36                    4814 	.db #0x36	; 54	'6'
      001626 00                    4815 	.db #0x00	; 0
      001627 00                    4816 	.db #0x00	; 0
      001628 00                    4817 	.db #0x00	; 0
      001629 56                    4818 	.db #0x56	; 86	'V'
      00162A 36                    4819 	.db #0x36	; 54	'6'
      00162B 00                    4820 	.db #0x00	; 0
      00162C 00                    4821 	.db #0x00	; 0
      00162D 00                    4822 	.db #0x00	; 0
      00162E 08                    4823 	.db #0x08	; 8
      00162F 14                    4824 	.db #0x14	; 20
      001630 22                    4825 	.db #0x22	; 34
      001631 41                    4826 	.db #0x41	; 65	'A'
      001632 14                    4827 	.db #0x14	; 20
      001633 14                    4828 	.db #0x14	; 20
      001634 14                    4829 	.db #0x14	; 20
      001635 14                    4830 	.db #0x14	; 20
      001636 14                    4831 	.db #0x14	; 20
      001637 41                    4832 	.db #0x41	; 65	'A'
      001638 22                    4833 	.db #0x22	; 34
      001639 14                    4834 	.db #0x14	; 20
      00163A 08                    4835 	.db #0x08	; 8
      00163B 00                    4836 	.db #0x00	; 0
      00163C 02                    4837 	.db #0x02	; 2
      00163D 01                    4838 	.db #0x01	; 1
      00163E 51                    4839 	.db #0x51	; 81	'Q'
      00163F 09                    4840 	.db #0x09	; 9
      001640 06                    4841 	.db #0x06	; 6
      001641 32                    4842 	.db #0x32	; 50	'2'
      001642 49                    4843 	.db #0x49	; 73	'I'
      001643 79                    4844 	.db #0x79	; 121	'y'
      001644 41                    4845 	.db #0x41	; 65	'A'
      001645 3E                    4846 	.db #0x3e	; 62
      001646 7E                    4847 	.db #0x7e	; 126
      001647 11                    4848 	.db #0x11	; 17
      001648 11                    4849 	.db #0x11	; 17
      001649 11                    4850 	.db #0x11	; 17
      00164A 7E                    4851 	.db #0x7e	; 126
      00164B 7F                    4852 	.db #0x7f	; 127
      00164C 49                    4853 	.db #0x49	; 73	'I'
      00164D 49                    4854 	.db #0x49	; 73	'I'
      00164E 49                    4855 	.db #0x49	; 73	'I'
      00164F 36                    4856 	.db #0x36	; 54	'6'
      001650 3E                    4857 	.db #0x3e	; 62
      001651 41                    4858 	.db #0x41	; 65	'A'
      001652 41                    4859 	.db #0x41	; 65	'A'
      001653 41                    4860 	.db #0x41	; 65	'A'
      001654 22                    4861 	.db #0x22	; 34
      001655 7F                    4862 	.db #0x7f	; 127
      001656 41                    4863 	.db #0x41	; 65	'A'
      001657 41                    4864 	.db #0x41	; 65	'A'
      001658 22                    4865 	.db #0x22	; 34
      001659 1C                    4866 	.db #0x1c	; 28
      00165A 7F                    4867 	.db #0x7f	; 127
      00165B 49                    4868 	.db #0x49	; 73	'I'
      00165C 49                    4869 	.db #0x49	; 73	'I'
      00165D 49                    4870 	.db #0x49	; 73	'I'
      00165E 41                    4871 	.db #0x41	; 65	'A'
      00165F 7F                    4872 	.db #0x7f	; 127
      001660 09                    4873 	.db #0x09	; 9
      001661 09                    4874 	.db #0x09	; 9
      001662 01                    4875 	.db #0x01	; 1
      001663 01                    4876 	.db #0x01	; 1
      001664 3E                    4877 	.db #0x3e	; 62
      001665 41                    4878 	.db #0x41	; 65	'A'
      001666 41                    4879 	.db #0x41	; 65	'A'
      001667 51                    4880 	.db #0x51	; 81	'Q'
      001668 32                    4881 	.db #0x32	; 50	'2'
      001669 7F                    4882 	.db #0x7f	; 127
      00166A 08                    4883 	.db #0x08	; 8
      00166B 08                    4884 	.db #0x08	; 8
      00166C 08                    4885 	.db #0x08	; 8
      00166D 7F                    4886 	.db #0x7f	; 127
      00166E 00                    4887 	.db #0x00	; 0
      00166F 41                    4888 	.db #0x41	; 65	'A'
      001670 7F                    4889 	.db #0x7f	; 127
      001671 41                    4890 	.db #0x41	; 65	'A'
      001672 00                    4891 	.db #0x00	; 0
      001673 20                    4892 	.db #0x20	; 32
      001674 40                    4893 	.db #0x40	; 64
      001675 41                    4894 	.db #0x41	; 65	'A'
      001676 3F                    4895 	.db #0x3f	; 63
      001677 01                    4896 	.db #0x01	; 1
      001678 7F                    4897 	.db #0x7f	; 127
      001679 08                    4898 	.db #0x08	; 8
      00167A 14                    4899 	.db #0x14	; 20
      00167B 22                    4900 	.db #0x22	; 34
      00167C 41                    4901 	.db #0x41	; 65	'A'
      00167D 7F                    4902 	.db #0x7f	; 127
      00167E 40                    4903 	.db #0x40	; 64
      00167F 40                    4904 	.db #0x40	; 64
      001680 40                    4905 	.db #0x40	; 64
      001681 40                    4906 	.db #0x40	; 64
      001682 7F                    4907 	.db #0x7f	; 127
      001683 02                    4908 	.db #0x02	; 2
      001684 04                    4909 	.db #0x04	; 4
      001685 02                    4910 	.db #0x02	; 2
      001686 7F                    4911 	.db #0x7f	; 127
      001687 7F                    4912 	.db #0x7f	; 127
      001688 04                    4913 	.db #0x04	; 4
      001689 08                    4914 	.db #0x08	; 8
      00168A 10                    4915 	.db #0x10	; 16
      00168B 7F                    4916 	.db #0x7f	; 127
      00168C 3E                    4917 	.db #0x3e	; 62
      00168D 41                    4918 	.db #0x41	; 65	'A'
      00168E 41                    4919 	.db #0x41	; 65	'A'
      00168F 41                    4920 	.db #0x41	; 65	'A'
      001690 3E                    4921 	.db #0x3e	; 62
      001691 7F                    4922 	.db #0x7f	; 127
      001692 09                    4923 	.db #0x09	; 9
      001693 09                    4924 	.db #0x09	; 9
      001694 09                    4925 	.db #0x09	; 9
      001695 06                    4926 	.db #0x06	; 6
      001696 3E                    4927 	.db #0x3e	; 62
      001697 41                    4928 	.db #0x41	; 65	'A'
      001698 51                    4929 	.db #0x51	; 81	'Q'
      001699 21                    4930 	.db #0x21	; 33
      00169A 5E                    4931 	.db #0x5e	; 94
      00169B 7F                    4932 	.db #0x7f	; 127
      00169C 09                    4933 	.db #0x09	; 9
      00169D 19                    4934 	.db #0x19	; 25
      00169E 29                    4935 	.db #0x29	; 41
      00169F 46                    4936 	.db #0x46	; 70	'F'
      0016A0 46                    4937 	.db #0x46	; 70	'F'
      0016A1 49                    4938 	.db #0x49	; 73	'I'
      0016A2 49                    4939 	.db #0x49	; 73	'I'
      0016A3 49                    4940 	.db #0x49	; 73	'I'
      0016A4 31                    4941 	.db #0x31	; 49	'1'
      0016A5 01                    4942 	.db #0x01	; 1
      0016A6 01                    4943 	.db #0x01	; 1
      0016A7 7F                    4944 	.db #0x7f	; 127
      0016A8 01                    4945 	.db #0x01	; 1
      0016A9 01                    4946 	.db #0x01	; 1
      0016AA 3F                    4947 	.db #0x3f	; 63
      0016AB 40                    4948 	.db #0x40	; 64
      0016AC 40                    4949 	.db #0x40	; 64
      0016AD 40                    4950 	.db #0x40	; 64
      0016AE 3F                    4951 	.db #0x3f	; 63
      0016AF 1F                    4952 	.db #0x1f	; 31
      0016B0 20                    4953 	.db #0x20	; 32
      0016B1 40                    4954 	.db #0x40	; 64
      0016B2 20                    4955 	.db #0x20	; 32
      0016B3 1F                    4956 	.db #0x1f	; 31
      0016B4 7F                    4957 	.db #0x7f	; 127
      0016B5 20                    4958 	.db #0x20	; 32
      0016B6 18                    4959 	.db #0x18	; 24
      0016B7 20                    4960 	.db #0x20	; 32
      0016B8 7F                    4961 	.db #0x7f	; 127
      0016B9 63                    4962 	.db #0x63	; 99	'c'
      0016BA 14                    4963 	.db #0x14	; 20
      0016BB 08                    4964 	.db #0x08	; 8
      0016BC 14                    4965 	.db #0x14	; 20
      0016BD 63                    4966 	.db #0x63	; 99	'c'
      0016BE 03                    4967 	.db #0x03	; 3
      0016BF 04                    4968 	.db #0x04	; 4
      0016C0 78                    4969 	.db #0x78	; 120	'x'
      0016C1 04                    4970 	.db #0x04	; 4
      0016C2 03                    4971 	.db #0x03	; 3
      0016C3 61                    4972 	.db #0x61	; 97	'a'
      0016C4 51                    4973 	.db #0x51	; 81	'Q'
      0016C5 49                    4974 	.db #0x49	; 73	'I'
      0016C6 45                    4975 	.db #0x45	; 69	'E'
      0016C7 43                    4976 	.db #0x43	; 67	'C'
      0016C8 00                    4977 	.db #0x00	; 0
      0016C9 00                    4978 	.db #0x00	; 0
      0016CA 7F                    4979 	.db #0x7f	; 127
      0016CB 41                    4980 	.db #0x41	; 65	'A'
      0016CC 41                    4981 	.db #0x41	; 65	'A'
      0016CD 02                    4982 	.db #0x02	; 2
      0016CE 04                    4983 	.db #0x04	; 4
      0016CF 08                    4984 	.db #0x08	; 8
      0016D0 10                    4985 	.db #0x10	; 16
      0016D1 20                    4986 	.db #0x20	; 32
      0016D2 41                    4987 	.db #0x41	; 65	'A'
      0016D3 41                    4988 	.db #0x41	; 65	'A'
      0016D4 7F                    4989 	.db #0x7f	; 127
      0016D5 00                    4990 	.db #0x00	; 0
      0016D6 00                    4991 	.db #0x00	; 0
      0016D7 04                    4992 	.db #0x04	; 4
      0016D8 02                    4993 	.db #0x02	; 2
      0016D9 01                    4994 	.db #0x01	; 1
      0016DA 02                    4995 	.db #0x02	; 2
      0016DB 04                    4996 	.db #0x04	; 4
      0016DC 40                    4997 	.db #0x40	; 64
      0016DD 40                    4998 	.db #0x40	; 64
      0016DE 40                    4999 	.db #0x40	; 64
      0016DF 40                    5000 	.db #0x40	; 64
      0016E0 40                    5001 	.db #0x40	; 64
      0016E1 00                    5002 	.db #0x00	; 0
      0016E2 01                    5003 	.db #0x01	; 1
      0016E3 02                    5004 	.db #0x02	; 2
      0016E4 04                    5005 	.db #0x04	; 4
      0016E5 00                    5006 	.db #0x00	; 0
      0016E6 20                    5007 	.db #0x20	; 32
      0016E7 54                    5008 	.db #0x54	; 84	'T'
      0016E8 54                    5009 	.db #0x54	; 84	'T'
      0016E9 54                    5010 	.db #0x54	; 84	'T'
      0016EA 78                    5011 	.db #0x78	; 120	'x'
      0016EB 7F                    5012 	.db #0x7f	; 127
      0016EC 48                    5013 	.db #0x48	; 72	'H'
      0016ED 44                    5014 	.db #0x44	; 68	'D'
      0016EE 44                    5015 	.db #0x44	; 68	'D'
      0016EF 38                    5016 	.db #0x38	; 56	'8'
      0016F0 38                    5017 	.db #0x38	; 56	'8'
      0016F1 44                    5018 	.db #0x44	; 68	'D'
      0016F2 44                    5019 	.db #0x44	; 68	'D'
      0016F3 44                    5020 	.db #0x44	; 68	'D'
      0016F4 20                    5021 	.db #0x20	; 32
      0016F5 38                    5022 	.db #0x38	; 56	'8'
      0016F6 44                    5023 	.db #0x44	; 68	'D'
      0016F7 44                    5024 	.db #0x44	; 68	'D'
      0016F8 48                    5025 	.db #0x48	; 72	'H'
      0016F9 7F                    5026 	.db #0x7f	; 127
      0016FA 38                    5027 	.db #0x38	; 56	'8'
      0016FB 54                    5028 	.db #0x54	; 84	'T'
      0016FC 54                    5029 	.db #0x54	; 84	'T'
      0016FD 54                    5030 	.db #0x54	; 84	'T'
      0016FE 18                    5031 	.db #0x18	; 24
      0016FF 08                    5032 	.db #0x08	; 8
      001700 7E                    5033 	.db #0x7e	; 126
      001701 09                    5034 	.db #0x09	; 9
      001702 01                    5035 	.db #0x01	; 1
      001703 02                    5036 	.db #0x02	; 2
      001704 08                    5037 	.db #0x08	; 8
      001705 14                    5038 	.db #0x14	; 20
      001706 54                    5039 	.db #0x54	; 84	'T'
      001707 54                    5040 	.db #0x54	; 84	'T'
      001708 3C                    5041 	.db #0x3c	; 60
      001709 7F                    5042 	.db #0x7f	; 127
      00170A 08                    5043 	.db #0x08	; 8
      00170B 04                    5044 	.db #0x04	; 4
      00170C 04                    5045 	.db #0x04	; 4
      00170D 78                    5046 	.db #0x78	; 120	'x'
      00170E 00                    5047 	.db #0x00	; 0
      00170F 44                    5048 	.db #0x44	; 68	'D'
      001710 7D                    5049 	.db #0x7d	; 125
      001711 40                    5050 	.db #0x40	; 64
      001712 00                    5051 	.db #0x00	; 0
      001713 20                    5052 	.db #0x20	; 32
      001714 40                    5053 	.db #0x40	; 64
      001715 44                    5054 	.db #0x44	; 68	'D'
      001716 3D                    5055 	.db #0x3d	; 61
      001717 00                    5056 	.db #0x00	; 0
      001718 00                    5057 	.db #0x00	; 0
      001719 7F                    5058 	.db #0x7f	; 127
      00171A 10                    5059 	.db #0x10	; 16
      00171B 28                    5060 	.db #0x28	; 40
      00171C 44                    5061 	.db #0x44	; 68	'D'
      00171D 00                    5062 	.db #0x00	; 0
      00171E 41                    5063 	.db #0x41	; 65	'A'
      00171F 7F                    5064 	.db #0x7f	; 127
      001720 40                    5065 	.db #0x40	; 64
      001721 00                    5066 	.db #0x00	; 0
      001722 7C                    5067 	.db #0x7c	; 124
      001723 04                    5068 	.db #0x04	; 4
      001724 18                    5069 	.db #0x18	; 24
      001725 04                    5070 	.db #0x04	; 4
      001726 78                    5071 	.db #0x78	; 120	'x'
      001727 7C                    5072 	.db #0x7c	; 124
      001728 08                    5073 	.db #0x08	; 8
      001729 04                    5074 	.db #0x04	; 4
      00172A 04                    5075 	.db #0x04	; 4
      00172B 78                    5076 	.db #0x78	; 120	'x'
      00172C 38                    5077 	.db #0x38	; 56	'8'
      00172D 44                    5078 	.db #0x44	; 68	'D'
      00172E 44                    5079 	.db #0x44	; 68	'D'
      00172F 44                    5080 	.db #0x44	; 68	'D'
      001730 38                    5081 	.db #0x38	; 56	'8'
      001731 7C                    5082 	.db #0x7c	; 124
      001732 14                    5083 	.db #0x14	; 20
      001733 14                    5084 	.db #0x14	; 20
      001734 14                    5085 	.db #0x14	; 20
      001735 08                    5086 	.db #0x08	; 8
      001736 08                    5087 	.db #0x08	; 8
      001737 14                    5088 	.db #0x14	; 20
      001738 14                    5089 	.db #0x14	; 20
      001739 18                    5090 	.db #0x18	; 24
      00173A 7C                    5091 	.db #0x7c	; 124
      00173B 7C                    5092 	.db #0x7c	; 124
      00173C 08                    5093 	.db #0x08	; 8
      00173D 04                    5094 	.db #0x04	; 4
      00173E 04                    5095 	.db #0x04	; 4
      00173F 08                    5096 	.db #0x08	; 8
      001740 48                    5097 	.db #0x48	; 72	'H'
      001741 54                    5098 	.db #0x54	; 84	'T'
      001742 54                    5099 	.db #0x54	; 84	'T'
      001743 54                    5100 	.db #0x54	; 84	'T'
      001744 20                    5101 	.db #0x20	; 32
      001745 04                    5102 	.db #0x04	; 4
      001746 3F                    5103 	.db #0x3f	; 63
      001747 44                    5104 	.db #0x44	; 68	'D'
      001748 40                    5105 	.db #0x40	; 64
      001749 20                    5106 	.db #0x20	; 32
      00174A 3C                    5107 	.db #0x3c	; 60
      00174B 40                    5108 	.db #0x40	; 64
      00174C 40                    5109 	.db #0x40	; 64
      00174D 20                    5110 	.db #0x20	; 32
      00174E 7C                    5111 	.db #0x7c	; 124
      00174F 1C                    5112 	.db #0x1c	; 28
      001750 20                    5113 	.db #0x20	; 32
      001751 40                    5114 	.db #0x40	; 64
      001752 20                    5115 	.db #0x20	; 32
      001753 1C                    5116 	.db #0x1c	; 28
      001754 3C                    5117 	.db #0x3c	; 60
      001755 40                    5118 	.db #0x40	; 64
      001756 30                    5119 	.db #0x30	; 48	'0'
      001757 40                    5120 	.db #0x40	; 64
      001758 3C                    5121 	.db #0x3c	; 60
      001759 44                    5122 	.db #0x44	; 68	'D'
      00175A 28                    5123 	.db #0x28	; 40
      00175B 10                    5124 	.db #0x10	; 16
      00175C 28                    5125 	.db #0x28	; 40
      00175D 44                    5126 	.db #0x44	; 68	'D'
      00175E 0C                    5127 	.db #0x0c	; 12
      00175F 50                    5128 	.db #0x50	; 80	'P'
      001760 50                    5129 	.db #0x50	; 80	'P'
      001761 50                    5130 	.db #0x50	; 80	'P'
      001762 3C                    5131 	.db #0x3c	; 60
      001763 44                    5132 	.db #0x44	; 68	'D'
      001764 64                    5133 	.db #0x64	; 100	'd'
      001765 54                    5134 	.db #0x54	; 84	'T'
      001766 4C                    5135 	.db #0x4c	; 76	'L'
      001767 44                    5136 	.db #0x44	; 68	'D'
      001768 00                    5137 	.db #0x00	; 0
      001769 08                    5138 	.db #0x08	; 8
      00176A 36                    5139 	.db #0x36	; 54	'6'
      00176B 41                    5140 	.db #0x41	; 65	'A'
      00176C 00                    5141 	.db #0x00	; 0
      00176D 00                    5142 	.db #0x00	; 0
      00176E 00                    5143 	.db #0x00	; 0
      00176F 7F                    5144 	.db #0x7f	; 127
      001770 00                    5145 	.db #0x00	; 0
      001771 00                    5146 	.db #0x00	; 0
      001772 00                    5147 	.db #0x00	; 0
      001773 41                    5148 	.db #0x41	; 65	'A'
      001774 36                    5149 	.db #0x36	; 54	'6'
      001775 08                    5150 	.db #0x08	; 8
      001776 00                    5151 	.db #0x00	; 0
      001777 08                    5152 	.db #0x08	; 8
      001778 08                    5153 	.db #0x08	; 8
      001779 2A                    5154 	.db #0x2a	; 42
      00177A 1C                    5155 	.db #0x1c	; 28
      00177B 08                    5156 	.db #0x08	; 8
      00177C 08                    5157 	.db #0x08	; 8
      00177D 1C                    5158 	.db #0x1c	; 28
      00177E 2A                    5159 	.db #0x2a	; 42
      00177F 08                    5160 	.db #0x08	; 8
      001780 08                    5161 	.db #0x08	; 8
      001781 00                    5162 	.db #0x00	; 0
      001782 07                    5163 	.db #0x07	; 7
      001783 05                    5164 	.db #0x05	; 5
      001784 07                    5165 	.db #0x07	; 7
      001785 00                    5166 	.db #0x00	; 0
                           0001E5  5167 Fmain$__str_0$0$0 == .
      001786                       5168 ___str_0:
      001786 02                    5169 	.db 0x02
      001787 20 45 52 52 4F 3A 20  5170 	.ascii " ERRO: mem=%05d"
             6D 65 6D 3D 25 30 35
             64
      001796 00                    5171 	.db 0x00
                           0001F6  5172 Fmain$__str_1$0$0 == .
      001797                       5173 ___str_1:
      001797 02                    5174 	.db 0x02
      001798 20 69 20 3D 20 25 30  5175 	.ascii " i = %05d"
             35 64
      0017A1 00                    5176 	.db 0x00
                           000201  5177 Fmain$__str_2$0$0 == .
      0017A2                       5178 ___str_2:
      0017A2 20 25 30 32 64 2F 25  5179 	.ascii " %02d/%02d/2%03d | %02d:%02d:%02d |"
             30 32 64 2F 32 25 30
             33 64 20 7C 20 25 30
             32 64 3A 25 30 32 64
             3A 25 30 32 64 20 7C
      0017C5 00                    5180 	.db 0x00
                           000225  5181 Fmain$__str_3$0$0 == .
      0017C6                       5182 ___str_3:
      0017C6 01                    5183 	.db 0x01
      0017C7 20 25 30 32 64 2F 25  5184 	.ascii " %02d/%02d/2%03d "
             30 32 64 2F 32 25 30
             33 64 20
      0017D8 02                    5185 	.db 0x02
      0017D9 20 25 30 32 64 3A 25  5186 	.ascii " %02d:%02d:%02d"
             30 32 64 3A 25 30 32
             64
      0017E8 0A                    5187 	.db 0x0a
      0017E9 00                    5188 	.db 0x00
                           000249  5189 Fmain$__str_4$0$0 == .
      0017EA                       5190 ___str_4:
      0017EA 09                    5191 	.db 0x09
      0017EB 20                    5192 	.ascii " "
      0017EC 0A                    5193 	.db 0x0a
      0017ED 49 6D 70 72 69 6D 69  5194 	.ascii "Imprimindo amostras no terminal."
             6E 64 6F 20 61 6D 6F
             73 74 72 61 73 20 6E
             6F 20 74 65 72 6D 69
             6E 61 6C 2E
      00180D 0A                    5195 	.db 0x0a
      00180E 50 72 65 73 73 69 6F  5196 	.ascii "Pressione qualquer tecla"
             6E 65 20 71 75 61 6C
             71 75 65 72 20 74 65
             63 6C 61
      001826 20 70 61 72 61 20 73  5197 	.ascii " para sair."
             61 69 72 2E
      001831 0A                    5198 	.db 0x0a
      001832 00                    5199 	.db 0x00
                           000292  5200 Fmain$__str_5$0$0 == .
      001833                       5201 ___str_5:
      001833 25 30 32 64 2F 25 30  5202 	.ascii "%02d/%02d/2%03d | %02d:%02d:%02d |"
             32 64 2F 32 25 30 33
             64 20 7C 20 25 30 32
             64 3A 25 30 32 64 3A
             25 30 32 64 20 7C
      001855 00                    5203 	.db 0x00
                           0002B5  5204 Fmain$__str_6$0$0 == .
      001856                       5205 ___str_6:
      001856 20 55 6D 69 20 3D 20  5206 	.ascii " Umi = %2d %% | Temp = %2d "
             25 32 64 20 25 25 20
             7C 20 54 65 6D 70 20
             3D 20 25 32 64 20
      001871 B0                    5207 	.db 0xb0
      001872 43 20 7C 20 4C 75 7A  5208 	.ascii "C | Luz = %3.02f V | Chuva = %u"
             20 3D 20 25 33 2E 30
             32 66 20 56 20 7C 20
             43 68 75 76 61 20 3D
             20 25 75
      001891 0A                    5209 	.db 0x0a
      001892 00                    5210 	.db 0x00
                           0002F2  5211 Fmain$__str_7$0$0 == .
      001893                       5212 ___str_7:
      001893 09                    5213 	.db 0x09
      001894 20                    5214 	.ascii " "
      001895 0A                    5215 	.db 0x0a
      001896 49 6D 70 72 69 6D 69  5216 	.ascii "Imprimindo dados no GLCD."
             6E 64 6F 20 64 61 64
             6F 73 20 6E 6F 20 47
             4C 43 44 2E
      0018AF 0A                    5217 	.db 0x0a
      0018B0 50 72 65 73 73 69 6F  5218 	.ascii "Pressione qualquer tecla para s"
             6E 65 20 71 75 61 6C
             71 75 65 72 20 74 65
             63 6C 61 20 70 61 72
             61 20 73
      0018CF 61 69 72 2E           5219 	.ascii "air."
      0018D3 0A                    5220 	.db 0x0a
      0018D4 00                    5221 	.db 0x00
                           000334  5222 Fmain$__str_8$0$0 == .
      0018D5                       5223 ___str_8:
      0018D5 03                    5224 	.db 0x03
      0018D6 20 55 52 20 3D 20 25  5225 	.ascii " UR = %2d %%"
             32 64 20 25 25
      0018E2 00                    5226 	.db 0x00
                           000342  5227 Fmain$__str_9$0$0 == .
      0018E3                       5228 ___str_9:
      0018E3 04                    5229 	.db 0x04
      0018E4 20 54 65 6D 70 20 3D  5230 	.ascii " Temp = %2d "
             20 25 32 64 20
      0018F0 B0                    5231 	.db 0xb0
      0018F1 43                    5232 	.ascii "C"
      0018F2 00                    5233 	.db 0x00
                           000352  5234 Fmain$__str_10$0$0 == .
      0018F3                       5235 ___str_10:
      0018F3 05                    5236 	.db 0x05
      0018F4 20 4D 75 69 74 6F 20  5237 	.ascii " Muito claro"
             63 6C 61 72 6F
      001900 00                    5238 	.db 0x00
                           000360  5239 Fmain$__str_11$0$0 == .
      001901                       5240 ___str_11:
      001901 05                    5241 	.db 0x05
      001902 20 43 6C 61 72 6F     5242 	.ascii " Claro"
      001908 00                    5243 	.db 0x00
                           000368  5244 Fmain$__str_12$0$0 == .
      001909                       5245 ___str_12:
      001909 05                    5246 	.db 0x05
      00190A 20 45 73 63 75 72 6F  5247 	.ascii " Escuro"
      001911 00                    5248 	.db 0x00
                           000371  5249 Fmain$__str_13$0$0 == .
      001912                       5250 ___str_13:
      001912 05                    5251 	.db 0x05
      001913 20 4D 75 69 74 6F 20  5252 	.ascii " Muito escuro"
             65 73 63 75 72 6F
      001920 0A                    5253 	.db 0x0a
      001921 00                    5254 	.db 0x00
                           000381  5255 Fmain$__str_14$0$0 == .
      001922                       5256 ___str_14:
      001922 06                    5257 	.db 0x06
      001923 20 53 65 6D 20 63 68  5258 	.ascii " Sem chuva"
             75 76 61
      00192D 00                    5259 	.db 0x00
                           00038D  5260 Fmain$__str_15$0$0 == .
      00192E                       5261 ___str_15:
      00192E 06                    5262 	.db 0x06
      00192F 20 43 68 6F 76 65 6E  5263 	.ascii " Chovendo"
             64 6F
      001938 0A                    5264 	.db 0x0a
      001939 00                    5265 	.db 0x00
                           000399  5266 Fmain$__str_16$0$0 == .
      00193A                       5267 ___str_16:
      00193A 09                    5268 	.db 0x09
      00193B 20                    5269 	.ascii " "
      00193C 0A                    5270 	.db 0x0a
      00193D 00                    5271 	.db 0x00
                           00039D  5272 Fmain$__str_17$0$0 == .
      00193E                       5273 ___str_17:
      00193E 09                    5274 	.db 0x09
      00193F 20                    5275 	.ascii " "
      001940 0A                    5276 	.db 0x0a
      001941 49 6D 70 72 69 6D 69  5277 	.ascii "Imprimindo dados no terminal."
             6E 64 6F 20 64 61 64
             6F 73 20 6E 6F 20 74
             65 72 6D 69 6E 61 6C
             2E
      00195E 0A                    5278 	.db 0x0a
      00195F 50 72 65 73 73 69 6F  5279 	.ascii "Pressione qualquer tecla pa"
             6E 65 20 71 75 61 6C
             71 75 65 72 20 74 65
             63 6C 61 20 70 61
      00197A 72 61 20 73 61 69 72  5280 	.ascii "ra sair."
             2E
      001982 0A                    5281 	.db 0x0a
      001983 00                    5282 	.db 0x00
                           0003E3  5283 Fmain$__str_18$0$0 == .
      001984                       5284 ___str_18:
      001984 20 55 6D 69 20 3D 20  5285 	.ascii " Umi = %2d %% | Temp = %2d "
             25 32 64 20 25 25 20
             7C 20 54 65 6D 70 20
             3D 20 25 32 64 20
      00199F B0                    5286 	.db 0xb0
      0019A0 43 20 7C 20 4C 75 7A  5287 	.ascii "C | Luz = %3.02f V | Chuva = %u"
             20 3D 20 25 33 2E 30
             32 66 20 56 20 7C 20
             43 68 75 76 61 20 3D
             20 25 75
      0019BF 0D                    5288 	.db 0x0d
      0019C0 00                    5289 	.db 0x00
                           000420  5290 Fmain$__str_19$0$0 == .
      0019C1                       5291 ___str_19:
      0019C1 09                    5292 	.db 0x09
      0019C2 20                    5293 	.ascii " "
      0019C3 0A                    5294 	.db 0x0a
      0019C4 4D 45 4E 55 3A        5295 	.ascii "MENU:"
      0019C9 0A                    5296 	.db 0x0a
      0019CA 61 20 2D 20 4C 65 69  5297 	.ascii "a - Leitura no terminal"
             74 75 72 61 20 6E 6F
             20 74 65 72 6D 69 6E
             61 6C
      0019E1 0A                    5298 	.db 0x0a
      0019E2 62 20 2D 20 4C 65 69  5299 	.ascii "b - Leitura no GLCD"
             74 75 72 61 20 6E 6F
             20 47 4C 43 44
      0019F5 0A                    5300 	.db 0x0a
      0019F6 64 20 2D 20 49 6D 70  5301 	.ascii "d - Imp"
      0019FD 72 69 6D 65 20 61 6D  5302 	.ascii "rime amostras coletadas"
             6F 73 74 72 61 73 20
             63 6F 6C 65 74 61 64
             61 73
      001A14 0A                    5303 	.db 0x0a
      001A15 00                    5304 	.db 0x00
                           000475  5305 Fmain$__str_20$0$0 == .
      001A16                       5306 ___str_20:
      001A16 09                    5307 	.db 0x09
      001A17 20                    5308 	.ascii " "
      001A18 0A                    5309 	.db 0x0a
      001A19 44 45 46 41 55 4C 54  5310 	.ascii "DEFAULT"
      001A20 0A                    5311 	.db 0x0a
      001A21 00                    5312 	.db 0x00
                           000481  5313 Fmain$__str_21$0$0 == .
      001A22                       5314 ___str_21:
      001A22 09                    5315 	.db 0x09
      001A23 20                    5316 	.ascii " "
      001A24 0A                    5317 	.db 0x0a
      001A25 53 54 41 52 54        5318 	.ascii "START"
      001A2A 0A                    5319 	.db 0x0a
      001A2B 00                    5320 	.db 0x00
                                   5321 	.area XINIT   (CODE)
                                   5322 	.area CABS    (ABS,CODE)

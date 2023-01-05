```

undefined8 main(void)

{
  basic_istream<char,std--char_traits<char>> *this;
  int local_1c;
  int local_18;
  int local_14;
  char *local_10;
  
  local_14 = 0;
  local_18 = 0;
  local_1c = 0;
  operator<<<std--char_traits<char>>((basic_ostream *)cout,"Enter three numbers!\n");
  this = (basic_istream<char,std--char_traits<char>> *)
         operator>>((basic_istream<char,std--char_traits<char>> *)cin,&local_14);
  this = (basic_istream<char,std--char_traits<char>> *)operator>>(this,&local_18);
  operator>>(this,&local_1c);
  local_10 = (char *)gen(local_1c + local_14 + local_18);
  if (local_1c + local_14 + local_18 == 0x539) {
    operator<<<std--char_traits<char>>((basic_ostream *)cout,"easyctf{");
    print_ptr(local_10);
    puts("}");
  }
  else {
    operator<<<std--char_traits<char>>((basic_ostream *)cout,"nope.\n");
  }
  free(local_10);
  return 0;
}

```
```
undefined8 main(void)

{
  int iVar1;
  time_t tVar2;
  char *pcVar3;
  basic_ostream *this;
  long lVar4;
  uint uVar5;
  undefined8 *puVar6;
  undefined8 *puVar7;
  byte bVar8;
  int local_a8;
  int local_a4;
  uint local_a0;
  int local_9c;
  undefined8 local_98 [18];
  
  bVar8 = 0;
  primp();
  lVar4 = 0x11;
  puVar6 = &DAT_00400d80;
  puVar7 = local_98;
  while (lVar4 != 0) {
    lVar4 = lVar4 + -1;
    *puVar7 = *puVar6;
    puVar6 = puVar6 + (ulong)bVar8 * 0x1ffffffffffffffe + 1;
    puVar7 = puVar7 + (ulong)bVar8 * 0x1ffffffffffffffe + 1;
  }
  tVar2 = time((time_t *)0x0);
  srand((uint)tVar2);
  iVar1 = rand();
  uVar5 = (uint)(iVar1 >> 0x1f) >> 6;
  local_9c = (iVar1 + uVar5 & 0x3ffffff) - uVar5;
  local_a4 = 0;
  local_a8 = 0;
  while( true ) {
    if (0x16 < local_a4) {
      local_a4 = local_a4 + 1;
      this = operator<<<std--char_traits<char>>((basic_ostream *)cout,"no dice.");
      operator<<((basic_ostream<char,std--char_traits<char>> *)this,
                 _ZSt4endlIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_);
      return 0;
    }
    local_a4 = local_a4 + 1;
    operator<<<std--char_traits<char>>((basic_ostream *)cout,"Guess? ");
    operator>>((basic_istream<char,std--char_traits<char>> *)cin,&local_a8);
    if (local_a8 == local_9c) break;
    if (local_a8 < local_9c) {
      pcVar3 = "lo";
    }
    else {
      pcVar3 = "hi";
    }
    this = operator<<<std--char_traits<char>>((basic_ostream *)cout,pcVar3);
    operator<<((basic_ostream<char,std--char_traits<char>> *)this,
               _ZSt4endlIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_);
  }
  local_a0 = 0;
  while (local_a0 < 0x22) {
    operator<<<std--char_traits<char>>
              ((basic_ostream *)cout,
               (byte)*(undefined4 *)(c610 + (long)(int)local_a0 * 4) ^
               (byte)*(undefined4 *)((long)local_98 + (long)(int)local_a0 * 4));
    local_a0 = local_a0 + 1;
  }
  return 1;
}

```
```
Dump of assembler code for function main:
   0x0000000000400af8 <+0>:	push   rbp
   0x0000000000400af9 <+1>:	mov    rbp,rsp
   0x0000000000400afc <+4>:	sub    rsp,0xa0
   0x0000000000400b03 <+11>:	call   0x400a7e <primp()>
   0x0000000000400b08 <+16>:	lea    rdx,[rbp-0x90]
   0x0000000000400b0f <+23>:	mov    esi,0x400d80
   0x0000000000400b14 <+28>:	mov    eax,0x11
   0x0000000000400b19 <+33>:	mov    rdi,rdx
   0x0000000000400b1c <+36>:	mov    rcx,rax
   0x0000000000400b1f <+39>:	rep movs QWORD PTR es:[rdi],QWORD PTR ds:[rsi]
   0x0000000000400b22 <+42>:	mov    edi,0x0
   0x0000000000400b27 <+47>:	call   0x400930 <time@plt>
   0x0000000000400b2c <+52>:	mov    edi,eax
   0x0000000000400b2e <+54>:	call   0x4008f0 <srand@plt>
   0x0000000000400b33 <+59>:	call   0x400920 <rand@plt>
   0x0000000000400b38 <+64>:	cdq    
   0x0000000000400b39 <+65>:	shr    edx,0x6
   0x0000000000400b3c <+68>:	add    eax,edx
   0x0000000000400b3e <+70>:	and    eax,0x3ffffff
   0x0000000000400b43 <+75>:	sub    eax,edx
   0x0000000000400b45 <+77>:	mov    DWORD PTR [rbp-0x94],eax
   0x0000000000400b4b <+83>:	mov    DWORD PTR [rbp-0x9c],0x0
   0x0000000000400b55 <+93>:	mov    DWORD PTR [rbp-0xa0],0x0
   0x0000000000400b5f <+103>:	jmp    0x400c27 <main+303>
   0x0000000000400b64 <+108>:	mov    esi,0x400d60
   0x0000000000400b69 <+113>:	mov    edi,0x6021c0
   0x0000000000400b6e <+118>:	call   0x4008d0 <std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*)@plt>
   0x0000000000400b73 <+123>:	lea    rax,[rbp-0xa0]
   0x0000000000400b7a <+130>:	mov    rsi,rax
   0x0000000000400b7d <+133>:	mov    edi,0x6020a0
   0x0000000000400b82 <+138>:	call   0x4008e0 <std::istream::operator>>(int&)@plt>
   0x0000000000400b87 <+143>:	mov    eax,DWORD PTR [rbp-0xa0]
   0x0000000000400b8d <+149>:	cmp    eax,DWORD PTR [rbp-0x94]
   0x0000000000400b93 <+155>:	jne    0x400bf3 <main+251>
   0x0000000000400b95 <+157>:	mov    DWORD PTR [rbp-0x98],0x0
   0x0000000000400b9f <+167>:	jmp    0x400bd9 <main+225>
   0x0000000000400ba1 <+169>:	mov    eax,DWORD PTR [rbp-0x98]
   0x0000000000400ba7 <+175>:	cdqe   
   0x0000000000400ba9 <+177>:	mov    eax,DWORD PTR [rbp+rax*4-0x90]
   0x0000000000400bb0 <+184>:	mov    edx,eax
   0x0000000000400bb2 <+186>:	mov    eax,DWORD PTR [rbp-0x98]
   0x0000000000400bb8 <+192>:	cdqe   
   0x0000000000400bba <+194>:	mov    eax,DWORD PTR [rax*4+0x602300]
   0x0000000000400bc1 <+201>:	xor    eax,edx
   0x0000000000400bc3 <+203>:	movsx  eax,al
   0x0000000000400bc6 <+206>:	mov    esi,eax
   0x0000000000400bc8 <+208>:	mov    edi,0x6021c0
   0x0000000000400bcd <+213>:	call   0x4008b0 <std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char)@plt>
   0x0000000000400bd2 <+218>:	add    DWORD PTR [rbp-0x98],0x1
   0x0000000000400bd9 <+225>:	mov    eax,DWORD PTR [rbp-0x98]
   0x0000000000400bdf <+231>:	movsxd rdx,eax
   0x0000000000400be2 <+234>:	mov    eax,0x22
   0x0000000000400be7 <+239>:	cmp    rdx,rax
   0x0000000000400bea <+242>:	jb     0x400ba1 <main+169>
   0x0000000000400bec <+244>:	mov    eax,0x1
   0x0000000000400bf1 <+249>:	jmp    0x400c65 <main+365>
   0x0000000000400bf3 <+251>:	mov    eax,DWORD PTR [rbp-0xa0]
   0x0000000000400bf9 <+257>:	cmp    eax,DWORD PTR [rbp-0x94]
   0x0000000000400bff <+263>:	jge    0x400c08 <main+272>
   0x0000000000400c01 <+265>:	mov    eax,0x400d68
   0x0000000000400c06 <+270>:	jmp    0x400c0d <main+277>
   0x0000000000400c08 <+272>:	mov    eax,0x400d6b
   0x0000000000400c0d <+277>:	mov    rsi,rax
   0x0000000000400c10 <+280>:	mov    edi,0x6021c0
   0x0000000000400c15 <+285>:	call   0x4008d0 <std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*)@plt>
   0x0000000000400c1a <+290>:	mov    esi,0x400910
   0x0000000000400c1f <+295>:	mov    rdi,rax
   0x0000000000400c22 <+298>:	call   0x400900 <std::ostream::operator<<(std::ostream& (*)(std::ostream&))@plt>
   0x0000000000400c27 <+303>:	mov    eax,DWORD PTR [rbp-0x9c]
   0x0000000000400c2d <+309>:	lea    edx,[rax+0x1]
   0x0000000000400c30 <+312>:	mov    DWORD PTR [rbp-0x9c],edx
   0x0000000000400c36 <+318>:	cmp    eax,0x16
   0x0000000000400c39 <+321>:	setle  al
   0x0000000000400c3c <+324>:	test   al,al
   0x0000000000400c3e <+326>:	jne    0x400b64 <main+108>
   0x0000000000400c44 <+332>:	mov    esi,0x400d6e
   0x0000000000400c49 <+337>:	mov    edi,0x6021c0
   0x0000000000400c4e <+342>:	call   0x4008d0 <std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*)@plt>
   0x0000000000400c53 <+347>:	mov    esi,0x400910
   0x0000000000400c58 <+352>:	mov    rdi,rax
   0x0000000000400c5b <+355>:	call   0x400900 <std::ostream::operator<<(std::ostream& (*)(std::ostream&))@plt>
   0x0000000000400c60 <+360>:	mov    eax,0x0
   0x0000000000400c65 <+365>:	leave  
   0x0000000000400c66 <+366>:	ret    
End of assembler dump.

```

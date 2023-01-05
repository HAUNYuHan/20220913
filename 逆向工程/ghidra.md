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

# Comparing `tmp/pyaon-1.1.6-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/pyaon-1.1.7-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 95963 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-10 03:00 pyaon-1.1.6.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-10 03:00 pyaon.libs/
--rwxr-xr-x  2.0 unx   229384 b- defN 23-Jul-10 03:00 pyaon.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-10 03:00 pyaon.pyi
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-10 03:00 pyaon-1.1.6.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1684 b- defN 23-Jul-10 03:00 pyaon-1.1.6.dist-info/LICENSE-3RD-PARTY
--rw-rw-r--  2.0 unx      554 b- defN 23-Jul-10 03:00 pyaon-1.1.6.dist-info/RECORD
--rw-r--r--  2.0 unx      162 b- defN 23-Jul-10 03:00 pyaon-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx     1746 b- defN 23-Jul-10 03:00 pyaon-1.1.6.dist-info/METADATA
-9 files, 233727 bytes uncompressed, 94781 bytes compressed:  59.4%
+Zip file size: 95970 bytes, number of entries: 9
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-10 03:27 pyaon-1.1.7.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-10 03:27 pyaon.libs/
+-rwxr-xr-x  2.0 unx   229384 b- defN 23-Jul-10 03:27 pyaon.pypy39-pp73-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-10 03:27 pyaon.pyi
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-10 03:27 pyaon-1.1.7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1684 b- defN 23-Jul-10 03:27 pyaon-1.1.7.dist-info/LICENSE-3RD-PARTY
+-rw-rw-r--  2.0 unx      554 b- defN 23-Jul-10 03:27 pyaon-1.1.7.dist-info/RECORD
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-10 03:27 pyaon-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1746 b- defN 23-Jul-10 03:27 pyaon-1.1.7.dist-info/METADATA
+9 files, 233740 bytes uncompressed, 94788 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: pyaon-1.1.6.dist-info/
+Filename: pyaon-1.1.7.dist-info/
 Comment: 
 
 Filename: pyaon.libs/
 Comment: 
 
 Filename: pyaon.pypy39-pp73-x86_64-linux-gnu.so
 Comment: 
 
 Filename: pyaon.pyi
 Comment: 
 
-Filename: pyaon-1.1.6.dist-info/top_level.txt
+Filename: pyaon-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaon-1.1.6.dist-info/LICENSE-3RD-PARTY
+Filename: pyaon-1.1.7.dist-info/LICENSE-3RD-PARTY
 Comment: 
 
-Filename: pyaon-1.1.6.dist-info/RECORD
+Filename: pyaon-1.1.7.dist-info/RECORD
 Comment: 
 
-Filename: pyaon-1.1.6.dist-info/WHEEL
+Filename: pyaon-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyaon-1.1.6.dist-info/METADATA
+Filename: pyaon-1.1.7.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## pyaon.pypy39-pp73-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a87e7aa8d47985d8642e1fb36d20f2ed99e6c2f9
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: f9649f4aea6ca13e258f08e61a567f20917c0a7c
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4060,15 +4060,15 @@
 	call   ec60 <__cxa_end_catch@plt>
 	jmp    22b85 <std::string::swap(std::string&)@@Base+0x5da5>
 	mov    %rax,%rbp
 	call   ec60 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   edb0 <_Unwind_Resume@plt>
 	nop
-	lea    0x1b081(%rip),%rdi        
+	lea    0x1b089(%rip),%rdi        
 	call   f370 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x440>
 	call   ecf0 <__cxa_begin_catch@plt>
 	mov    %r12,%rdi
 	call   23d00 <std::string::swap(std::string&)@@Base+0x6f20>
 	call   e330 <__cxa_rethrow@plt>
 	mov    %rax,%rbp
 	call   ec60 <__cxa_end_catch@plt>
@@ -4237,15 +4237,15 @@
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
 	jmp    135ae <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x467e>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   ed10 <std::basic_stringstream<char, std::char_traits<char>, std::allocator<char> >::~basic_stringstream()@plt>
 	jmp    134d3 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x45a3>
-	lea    0x1aee6(%rip),%rdi        
+	lea    0x1aeee(%rip),%rdi        
 	call   f370 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x440>
 	mov    $0x18,%edi
 	call   ea40 <__cxa_allocate_exception@plt>
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	call   f75e <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x82e>
 	lea    0x7915(%rip),%rdx        # 1af20 <std::string::_Rep::_S_create(unsigned long, unsigned long, std::allocator<char> const&)@@Base+0x6630>
@@ -4278,15 +4278,15 @@
 	mov    %r12,%rdi
 	call   edb0 <_Unwind_Resume@plt>
 	call   ecf0 <__cxa_begin_catch@plt>
 	mov    0x24860(%rip),%rdx        
 	mov    0x8(%rax),%rdi
 	mov    (%rdx),%rbp
 	call   1053c <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x160c>
-	lea    0x1acf5(%rip),%rsi        
+	lea    0x1acfb(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   15200 <std::string::_Rep::_S_create(unsigned long, unsigned long, std::allocator<char> const&)@@Base+0x910>
 	call   ec60 <__cxa_end_catch@plt>
 	xor    %r12d,%r12d
 	jmp    260b4 <PyInit_pyaon@@Base+0xb94>
 	mov    %rax,%rbp
 	jmp    136b5 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x4785>
@@ -4562,17 +4562,17 @@
 	mov    %r12,%rdi
 	call   eba0 <__cxa_throw@plt>
 	mov    %r12,%rdi
 	mov    %rax,%rbp
 	call   ea70 <__cxa_free_exception@plt>
 	jmp    13a83 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x4b53>
 	nop
-	lea    0x1ac29(%rip),%rdi        
+	lea    0x1ac31(%rip),%rdi        
 	call   f370 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x440>
-	lea    0x1ac4d(%rip),%rdi        
+	lea    0x1ac55(%rip),%rdi        
 	call   f370 <std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_replace_aux(unsigned long, unsigned long, unsigned long, char)@plt+0x440>
 	nop
 	lea    0x20(%rsp),%rdi
 	mov    %rax,%rbp
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	mov    0x30(%rsp),%rdi
 	mov    0x40(%rsp),%rsi
@@ -21341,15 +21341,15 @@
 	sub    $0x78,%rsp
 	call   e180 <PyPy_GetVersion@plt>
 	cmpb   $0x33,(%rax)
 	mov    %rax,%rcx
 	je     25570 <PyInit_pyaon@@Base+0x50>
 	mov    0x1299e(%rip),%rax        
 	lea    0x8e12(%rip),%rdx        
-	lea    0x8f10(%rip),%rsi        
+	lea    0x8f18(%rip),%rsi        
 	xor    %r12d,%r12d
 	mov    (%rax),%rdi
 	xor    %eax,%eax
 	call   e560 <PyPyErr_Format@plt>
 	add    $0x78,%rsp
 	mov    %r12,%rax
 	pop    %rbx
@@ -21386,15 +21386,15 @@
 	movups %xmm0,0x1329b(%rip)        # 388a8 <typeinfo for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0xcb8>
 	movups %xmm0,0x132a4(%rip)        # 388b8 <typeinfo for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0xcc8>
 	call   e640 <PyPyModule_Create2@plt>
 	test   %rax,%rax
 	je     261a0 <PyInit_pyaon@@Base+0xc80>
 	mov    %rax,0x28(%rsp)
 	lea    0x48(%rsp),%r14
-	lea    0x8ed5(%rip),%rsi        
+	lea    0x8edd(%rip),%rsi        
 	addq   $0x1,(%rax)
 	mov    %r14,%rdi
 	mov    %rax,0x58(%rsp)
 	lea    0x8961(%rip),%rax        
 	mov    %rax,0x60(%rsp)
 	lea    0x40(%rsp),%rax
 	mov    %rax,%rdx
@@ -21421,15 +21421,15 @@
 	jne    26409 <PyInit_pyaon@@Base+0xee9>
 	mov    %r14,%rdi
 	lea    0x30(%rsp),%r12
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	lea    0x68(%rsp),%rdi
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	lea    0x28(%rsp),%rax
-	lea    0x8e6b(%rip),%rcx        
+	lea    0x8e73(%rip),%rcx        
 	mov    %r12,%rdi
 	lea    0x8c7e(%rip),%rdx        
 	mov    %rax,%rsi
 	mov    %rax,0x8(%rsp)
 	call   20770 <std::string::swap(std::string&)@@Base+0x3990>
 	mov    0x12845(%rip),%rbx        
 	mov    0x30(%rsp),%rdi
@@ -21457,15 +21457,15 @@
 	mov    $0x1,%r10d
 	punpcklqdq %xmm1,%xmm0
 	mov    $0x1,%r8d
 	mov    %rbp,%rsi
 	mov    %r13,%rdi
 	movups %xmm0,0x30(%r15)
 	movq   0x10(%rsp),%xmm0
-	lea    0x8de3(%rip),%rax        
+	lea    0x8deb(%rip),%rax        
 	lea    0x935c(%rip),%rcx        # 2eaf8 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x58>
 	andb   $0x3f,0x59(%r15)
 	movq   %rax,%xmm3
 	lea    0x9353(%rip),%rdx        # 2eb00 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x60>
 	punpcklqdq %xmm2,%xmm0
 	mov    %r10w,0x5e(%r15)
 	movups %xmm0,0x70(%r15)
@@ -21510,15 +21510,15 @@
 	mov    0x50(%rsp),%r15
 	movq   %rcx,%xmm0
 	movq   %rax,%xmm4
 	mov    %r13,%rdi
 	mov    $0x2,%r9d
 	punpcklqdq %xmm4,%xmm0
 	andb   $0x3f,0x59(%r15)
-	lea    0x8d03(%rip),%rax        
+	lea    0x8d0b(%rip),%rax        
 	mov    $0x2,%r8d
 	movups %xmm0,0x30(%r15)
 	movq   0x18(%rsp),%xmm0
 	movq   %rax,%xmm5
 	lea    0x925e(%rip),%rcx        # 2eb18 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x78>
 	mov    %r9w,0x5e(%r15)
 	lea    0x925a(%rip),%rdx        # 2eb20 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x80>
@@ -21544,15 +21544,15 @@
 	mov    %r12,%rdi
 	call   25500 <std::string::swap(std::string&)@@Base+0x8720>
 	mov    %r13,%rdi
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	mov    %r12,%rdi
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	mov    0x8(%rsp),%rsi
-	lea    0x8c83(%rip),%rcx        
+	lea    0x8c8b(%rip),%rcx        
 	mov    %r12,%rdi
 	lea    0x8a28(%rip),%rdx        
 	call   20770 <std::string::swap(std::string&)@@Base+0x3990>
 	mov    0x30(%rsp),%rdi
 	lea    0x8a0d(%rip),%rsi        
 	addq   $0x1,(%rbx)
 	mov    %rbx,0x40(%rsp)
@@ -21571,15 +21571,15 @@
 	mov    %rbp,%rsi
 	mov    0x50(%rsp),%r15
 	movq   %rcx,%xmm0
 	movq   %rax,%xmm6
 	mov    $0x1,%r8d
 	mov    %r13,%rdi
 	punpcklqdq %xmm6,%xmm0
-	lea    0x8c28(%rip),%rax        
+	lea    0x8c30(%rip),%rax        
 	andb   $0x3f,0x59(%r15)
 	movups %xmm0,0x30(%r15)
 	movq   0x18(%rsp),%xmm0
 	movq   %rax,%xmm7
 	lea    0x9154(%rip),%rcx        # 2eb40 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0xa0>
 	mov    %r8w,0x5e(%r15)
 	lea    0x9168(%rip),%rdx        # 2eb60 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0xc0>
@@ -21635,15 +21635,15 @@
 	mov    0x50(%rsp),%r15
 	mov    $0x4,%edi
 	movq   %rcx,%xmm0
 	movq   %rax,%xmm1
 	mov    $0x4,%r8d
 	mov    %rbp,%rsi
 	punpcklqdq %xmm1,%xmm0
-	lea    0x8b16(%rip),%rax        
+	lea    0x8b1e(%rip),%rax        
 	andb   $0x3f,0x59(%r15)
 	movups %xmm0,0x30(%r15)
 	movq   0x18(%rsp),%xmm0
 	movq   %rax,%xmm2
 	lea    0x906a(%rip),%rcx        # 2eb90 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0xf0>
 	mov    %di,0x5e(%r15)
 	lea    0x906e(%rip),%rdx        # 2eba0 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x100>
@@ -21682,15 +21682,15 @@
 	je     26150 <PyInit_pyaon@@Base+0xc30>
 	mov    0x30(%rsp),%rdi
 	test   %rdi,%rdi
 	je     25bd7 <PyInit_pyaon@@Base+0x6b7>
 	subq   $0x1,(%rdi)
 	je     26140 <PyInit_pyaon@@Base+0xc20>
 	mov    0x8(%rsp),%rsi
-	lea    0x8a65(%rip),%rcx        
+	lea    0x8a6d(%rip),%rcx        
 	lea    0x8796(%rip),%rdx        
 	mov    %r12,%rdi
 	call   20770 <std::string::swap(std::string&)@@Base+0x3990>
 	mov    0x30(%rsp),%rdi
 	lea    0x876f(%rip),%rsi        
 	addq   $0x1,(%rbx)
 	mov    %rbx,0x40(%rsp)
@@ -21709,15 +21709,15 @@
 	mov    0x50(%rsp),%r15
 	mov    $0x1,%esi
 	movq   %rdx,%xmm0
 	movq   %rax,%xmm3
 	mov    $0x1,%r8d
 	mov    %r13,%rdi
 	punpcklqdq %xmm3,%xmm0
-	lea    0x8a08(%rip),%rax        
+	lea    0x8a10(%rip),%rax        
 	andb   $0x3f,0x59(%r15)
 	movups %xmm0,0x30(%r15)
 	movq   0x18(%rsp),%xmm0
 	movq   %rax,%xmm4
 	lea    0x8f4c(%rip),%rcx        # 2ebd8 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x138>
 	mov    %si,0x5e(%r15)
 	lea    0x8f48(%rip),%rdx        # 2ebe0 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x140>
@@ -21764,15 +21764,15 @@
 	mov    %rbp,%rsi
 	mov    0x50(%rsp),%r15
 	movq   %rcx,%xmm0
 	movq   %rax,%xmm5
 	mov    $0x2,%ecx
 	mov    $0x2,%r8d
 	punpcklqdq %xmm5,%xmm0
-	lea    0x891c(%rip),%rax        
+	lea    0x8924(%rip),%rax        
 	mov    %r13,%rdi
 	andb   $0x3f,0x59(%r15)
 	movups %xmm0,0x30(%r15)
 	movq   0x18(%rsp),%xmm0
 	movq   %rax,%xmm6
 	lea    0x8e5d(%rip),%rdx        # 2ec00 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x160>
 	mov    %cx,0x5e(%r15)
@@ -21799,17 +21799,17 @@
 	mov    %r12,%rdi
 	call   25500 <std::string::swap(std::string&)@@Base+0x8720>
 	mov    %r13,%rdi
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	mov    %r12,%rdi
 	call   226e0 <std::string::swap(std::string&)@@Base+0x5900>
 	mov    0x8(%rsp),%rsi
-	lea    0x889a(%rip),%rcx        
+	lea    0x88a2(%rip),%rcx        
 	mov    %r12,%rdi
-	lea    0x8548(%rip),%rdx        
+	lea    0x8550(%rip),%rdx        
 	call   20770 <std::string::swap(std::string&)@@Base+0x3990>
 	mov    0x30(%rsp),%rdi
 	lea    0x8524(%rip),%rsi        
 	addq   $0x1,(%rbx)
 	mov    %rbx,0x40(%rsp)
 	call   ec70 <PyPyObject_GetAttrString@plt>
 	mov    %rax,0x10(%rsp)
@@ -21826,15 +21826,15 @@
 	mov    %rbp,%rsi
 	mov    0x50(%rsp),%r15
 	movq   %rdx,%xmm0
 	movq   %rax,%xmm7
 	mov    $0x1,%edx
 	mov    $0x1,%r8d
 	punpcklqdq %xmm7,%xmm0
-	lea    0x883d(%rip),%rax        
+	lea    0x8845(%rip),%rax        
 	mov    %r13,%rdi
 	andb   $0x3f,0x59(%r15)
 	movups %xmm0,0x30(%r15)
 	movq   0x18(%rsp),%xmm0
 	movq   %rax,%xmm1
 	lea    0x8d46(%rip),%rcx        # 2ec20 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x180>
 	mov    %dx,0x5e(%r15)
@@ -21894,15 +21894,15 @@
 	mov    $0x2,%r8d
 	movq   %rcx,%xmm0
 	movq   %rax,%xmm2
 	mov    $0x2,%eax
 	andb   $0x3f,0x59(%rbx)
 	punpcklqdq %xmm2,%xmm0
 	mov    %ax,0x5e(%rbx)
-	lea    0x8720(%rip),%rax        
+	lea    0x8728(%rip),%rax        
 	lea    0x8c71(%rip),%rcx        # 2ec78 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x1d8>
 	movups %xmm0,0x30(%rbx)
 	movq   0x10(%rsp),%xmm0
 	movq   %rax,%xmm4
 	lea    0x8c63(%rip),%rdx        # 2ec80 <typeinfo name for void (*)(std::string const&, std::pair<unsigned long, std::map<unsigned long, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > >, std::less<unsigned long>, std::allocator<std::pair<unsigned long const, std::set<std::pair<unsigned long, unsigned long>, std::less<std::pair<unsigned long, unsigned long> >, std::allocator<std::pair<unsigned long, unsigned long> > > > > > > const&)@@Base+0x1e0>
 	punpcklqdq %xmm3,%xmm0
 	movups %xmm0,0x70(%rbx)
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -308,81 +308,81 @@
   0x0002e310 72656e63 655f6361 73745f65 72726f72 rence_cast_error
   0x0002e320 45007665 63746f72 3c626f6f 6c3e3a3a E.vector<bool>::
   0x0002e330 5f4d5f66 696c6c5f 696e7365 72740076 _M_fill_insert.v
   0x0002e340 6563746f 723c626f 6f6c3e3a 3a5f4d5f ector<bool>::_M_
   0x0002e350 696e7365 72745f61 75780033 2e390070 insert_aux.3.9.p
   0x0002e360 79616f6e 00736f72 74696e67 006c6f61 yaon.sorting.loa
   0x0002e370 64006475 6d70006b 6e617073 61636b00 d.dump.knapsack.
-  0x0002e380 68617368 696e6700 696e6974 69616c69 hashing.initiali
-  0x0002e390 7a617469 6f6e2066 61696c65 64000000 zation failed...
-  0x0002e3a0 70796269 6e643131 3a3a6465 7461696c pybind11::detail
-  0x0002e3b0 3a3a696e 7374616e 63653a3a 6765745f ::instance::get_
-  0x0002e3c0 76616c75 655f616e 645f686f 6c646572 value_and_holder
-  0x0002e3d0 3a207479 70652069 73206e6f 74206120 : type is not a 
-  0x0002e3e0 70796269 6e643131 20626173 65206f66 pybind11 base of
-  0x0002e3f0 20746865 20676976 656e2069 6e737461  the given insta
-  0x0002e400 6e636520 28236465 66696e65 20505942 nce (#define PYB
-  0x0002e410 494e4431 315f4445 5441494c 45445f45 IND11_DETAILED_E
-  0x0002e420 52524f52 5f4d4553 53414745 53206f72 RROR_MESSAGES or
-  0x0002e430 20636f6d 70696c65 20696e20 64656275  compile in debu
-  0x0002e440 67206d6f 64652066 6f722074 79706520 g mode for type 
-  0x0002e450 64657461 696c7329 00000000 00000000 details)........
-  0x0002e460 50797468 6f6e2076 65727369 6f6e206d Python version m
-  0x0002e470 69736d61 7463683a 206d6f64 756c6520 ismatch: module 
-  0x0002e480 77617320 636f6d70 696c6564 20666f72 was compiled for
-  0x0002e490 20507974 686f6e20 25732c20 62757420  Python %s, but 
-  0x0002e4a0 74686520 696e7465 72707265 74657220 the interpreter 
-  0x0002e4b0 76657273 696f6e20 69732069 6e636f6d version is incom
-  0x0002e4c0 70617469 626c653a 2025732e 00000000 patible: %s.....
-  0x0002e4d0 496e7465 726e616c 20657272 6f722069 Internal error i
-  0x0002e4e0 6e206d6f 64756c65 5f3a3a63 72656174 n module_::creat
-  0x0002e4f0 655f6578 74656e73 696f6e5f 6d6f6475 e_extension_modu
-  0x0002e500 6c652829 00000000 496e7465 72616374 le()....Interact
-  0x0002e510 20776974 68207468 6520414f 4e202841  with the AON (A
-  0x0002e520 6e647265 7a616f20 4f626a65 6374204e ndrezao Object N
-  0x0002e530 6f746174 696f6e29 2066696c 6520666f otation) file fo
-  0x0002e540 726d6174 00000000 50617273 6520616e rmat....Parse an
-  0x0002e550 64206475 6d702041 4f4e2066 696c6573 d dump AON files
-  0x0002e560 2028736f 7274696e 67207661 7269616e  (sorting varian
-  0x0002e570 74290000 00000000 4c6f6164 20616e20 t)......Load an 
-  0x0002e580 414f4e20 66696c65 2028736f 7274696e AON file (sortin
-  0x0002e590 67207661 7269616e 74290000 00000000 g variant)......
-  0x0002e5a0 44756d70 20616e20 414f4e20 66696c65 Dump an AON file
-  0x0002e5b0 2028736f 7274696e 67207661 7269616e  (sorting varian
-  0x0002e5c0 74290000 00000000 50617273 6520616e t)......Parse an
-  0x0002e5d0 64206475 6d702041 4f4e2066 696c6573 d dump AON files
-  0x0002e5e0 20286b6e 61707361 636b2076 61726961  (knapsack varia
-  0x0002e5f0 6e742900 00000000 4c6f6164 20616e20 nt).....Load an 
-  0x0002e600 414f4e20 66696c65 20286b6e 61707361 AON file (knapsa
-  0x0002e610 636b2076 61726961 6e742900 00000000 ck variant).....
-  0x0002e620 44756d70 20616e20 414f4e20 66696c65 Dump an AON file
-  0x0002e630 20286b6e 61707361 636b2076 61726961  (knapsack varia
-  0x0002e640 6e742900 00000000 50617273 6520616e nt).....Parse an
-  0x0002e650 64206475 6d702041 4f4e2066 696c6573 d dump AON files
-  0x0002e660 20286861 7368696e 67207661 7269616e  (hashing varian
-  0x0002e670 74290000 00000000 4c6f6164 20616e20 t)......Load an 
-  0x0002e680 414f4e20 66696c65 20286861 7368696e AON file (hashin
-  0x0002e690 67207661 7269616e 74290000 00000000 g variant)......
-  0x0002e6a0 44756d70 20616e20 414f4e20 66696c65 Dump an AON file
-  0x0002e6b0 20286861 7368696e 67207661 7269616e  (hashing varian
-  0x0002e6c0 74290000 00000000 50617273 6520616e t)......Parse an
-  0x0002e6d0 64206475 6d702041 4f4e2066 696c6573 d dump AON files
-  0x0002e6e0 20286772 61706820 76617269 616e7429  (graph variant)
-  0x0002e6f0 00000000 00000000 4c6f6164 20616e20 ........Load an 
-  0x0002e700 414f4e20 66696c65 20286772 61706820 AON file (graph 
-  0x0002e710 76617269 616e7429 00000000 00000000 variant)........
-  0x0002e720 44756d70 20616e20 414f4e20 66696c65 Dump an AON file
-  0x0002e730 20286772 61706820 76617269 616e7429  (graph variant)
-  0x0002e740 00000000 00000000 556e6578 70656374 ........Unexpect
-  0x0002e750 65642050 5942494e 4431315f 42595445 ed PYBIND11_BYTE
-  0x0002e760 535f4153 5f535452 494e4728 29206661 S_AS_STRING() fa
-  0x0002e770 696c7572 652e0000 556e6578 70656374 ilure...Unexpect
-  0x0002e780 65642050 79427974 65417272 61795f41 ed PyByteArray_A
-  0x0002e790 73537472 696e6728 29206661 696c7572 sString() failur
-  0x0002e7a0 652e0000 00000000 00000000 00000000 e...............
+  0x0002e380 68617368 696e6700 67726170 6800696e hashing.graph.in
+  0x0002e390 69746961 6c697a61 74696f6e 20666169 itialization fai
+  0x0002e3a0 6c656400 00000000 70796269 6e643131 led.....pybind11
+  0x0002e3b0 3a3a6465 7461696c 3a3a696e 7374616e ::detail::instan
+  0x0002e3c0 63653a3a 6765745f 76616c75 655f616e ce::get_value_an
+  0x0002e3d0 645f686f 6c646572 3a207479 70652069 d_holder: type i
+  0x0002e3e0 73206e6f 74206120 70796269 6e643131 s not a pybind11
+  0x0002e3f0 20626173 65206f66 20746865 20676976  base of the giv
+  0x0002e400 656e2069 6e737461 6e636520 28236465 en instance (#de
+  0x0002e410 66696e65 20505942 494e4431 315f4445 fine PYBIND11_DE
+  0x0002e420 5441494c 45445f45 52524f52 5f4d4553 TAILED_ERROR_MES
+  0x0002e430 53414745 53206f72 20636f6d 70696c65 SAGES or compile
+  0x0002e440 20696e20 64656275 67206d6f 64652066  in debug mode f
+  0x0002e450 6f722074 79706520 64657461 696c7329 or type details)
+  0x0002e460 00000000 00000000 50797468 6f6e2076 ........Python v
+  0x0002e470 65727369 6f6e206d 69736d61 7463683a ersion mismatch:
+  0x0002e480 206d6f64 756c6520 77617320 636f6d70  module was comp
+  0x0002e490 696c6564 20666f72 20507974 686f6e20 iled for Python 
+  0x0002e4a0 25732c20 62757420 74686520 696e7465 %s, but the inte
+  0x0002e4b0 72707265 74657220 76657273 696f6e20 rpreter version 
+  0x0002e4c0 69732069 6e636f6d 70617469 626c653a is incompatible:
+  0x0002e4d0 2025732e 00000000 496e7465 726e616c  %s.....Internal
+  0x0002e4e0 20657272 6f722069 6e206d6f 64756c65  error in module
+  0x0002e4f0 5f3a3a63 72656174 655f6578 74656e73 _::create_extens
+  0x0002e500 696f6e5f 6d6f6475 6c652829 00000000 ion_module()....
+  0x0002e510 496e7465 72616374 20776974 68207468 Interact with th
+  0x0002e520 6520414f 4e202841 6e647265 7a616f20 e AON (Andrezao 
+  0x0002e530 4f626a65 6374204e 6f746174 696f6e29 Object Notation)
+  0x0002e540 2066696c 6520666f 726d6174 00000000  file format....
+  0x0002e550 50617273 6520616e 64206475 6d702041 Parse and dump A
+  0x0002e560 4f4e2066 696c6573 2028736f 7274696e ON files (sortin
+  0x0002e570 67207661 7269616e 74290000 00000000 g variant)......
+  0x0002e580 4c6f6164 20616e20 414f4e20 66696c65 Load an AON file
+  0x0002e590 2028736f 7274696e 67207661 7269616e  (sorting varian
+  0x0002e5a0 74290000 00000000 44756d70 20616e20 t)......Dump an 
+  0x0002e5b0 414f4e20 66696c65 2028736f 7274696e AON file (sortin
+  0x0002e5c0 67207661 7269616e 74290000 00000000 g variant)......
+  0x0002e5d0 50617273 6520616e 64206475 6d702041 Parse and dump A
+  0x0002e5e0 4f4e2066 696c6573 20286b6e 61707361 ON files (knapsa
+  0x0002e5f0 636b2076 61726961 6e742900 00000000 ck variant).....
+  0x0002e600 4c6f6164 20616e20 414f4e20 66696c65 Load an AON file
+  0x0002e610 20286b6e 61707361 636b2076 61726961  (knapsack varia
+  0x0002e620 6e742900 00000000 44756d70 20616e20 nt).....Dump an 
+  0x0002e630 414f4e20 66696c65 20286b6e 61707361 AON file (knapsa
+  0x0002e640 636b2076 61726961 6e742900 00000000 ck variant).....
+  0x0002e650 50617273 6520616e 64206475 6d702041 Parse and dump A
+  0x0002e660 4f4e2066 696c6573 20286861 7368696e ON files (hashin
+  0x0002e670 67207661 7269616e 74290000 00000000 g variant)......
+  0x0002e680 4c6f6164 20616e20 414f4e20 66696c65 Load an AON file
+  0x0002e690 20286861 7368696e 67207661 7269616e  (hashing varian
+  0x0002e6a0 74290000 00000000 44756d70 20616e20 t)......Dump an 
+  0x0002e6b0 414f4e20 66696c65 20286861 7368696e AON file (hashin
+  0x0002e6c0 67207661 7269616e 74290000 00000000 g variant)......
+  0x0002e6d0 50617273 6520616e 64206475 6d702041 Parse and dump A
+  0x0002e6e0 4f4e2066 696c6573 20286772 61706820 ON files (graph 
+  0x0002e6f0 76617269 616e7429 00000000 00000000 variant)........
+  0x0002e700 4c6f6164 20616e20 414f4e20 66696c65 Load an AON file
+  0x0002e710 20286772 61706820 76617269 616e7429  (graph variant)
+  0x0002e720 00000000 00000000 44756d70 20616e20 ........Dump an 
+  0x0002e730 414f4e20 66696c65 20286772 61706820 AON file (graph 
+  0x0002e740 76617269 616e7429 00000000 00000000 variant)........
+  0x0002e750 556e6578 70656374 65642050 5942494e Unexpected PYBIN
+  0x0002e760 4431315f 42595445 535f4153 5f535452 D11_BYTES_AS_STR
+  0x0002e770 494e4728 29206661 696c7572 652e0000 ING() failure...
+  0x0002e780 556e6578 70656374 65642050 79427974 Unexpected PyByt
+  0x0002e790 65417272 61795f41 73537472 696e6728 eArray_AsString(
+  0x0002e7a0 29206661 696c7572 652e0000 00000000 ) failure.......
   0x0002e7b0 00000000 00000000 00000000 00000000 ................
   0x0002e7c0 46537436 76656374 6f724969 53614969 FSt6vectorIiSaIi
   0x0002e7d0 45455373 45000000 00000000 00000000 EESsE...........
   0x0002e7e0 46765253 74367665 63746f72 49695361 FvRSt6vectorIiSa
   0x0002e7f0 49694545 53734500 00000000 00000000 IiEESsE.........
   0x0002e800 46537435 7475706c 65494a6c 53743676 FSt5tupleIJlSt6v
   0x0002e810 6563746f 72496c53 61496c45 4553325f ectorIlSaIlEES2_
```

## pyaon.pyi

```diff
@@ -1,12 +1,13 @@
 """Interact with the AON (Andrezao Object Notation) file format"""
 from __future__ import annotations
 import pyaon
 import typing
 
 __all__ = [
+    "graph",
     "hashing",
     "knapsack",
     "sorting"
 ]
```

## Comparing `pyaon-1.1.6.dist-info/LICENSE-3RD-PARTY` & `pyaon-1.1.7.dist-info/LICENSE-3RD-PARTY`

 * *Files identical despite different names*

## Comparing `pyaon-1.1.6.dist-info/RECORD` & `pyaon-1.1.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pyaon.pypy39-pp73-x86_64-linux-gnu.so,sha256=bWZ6oODMagxgf-q2CUvXytqJtpjjWwlwAyqGOwh5MR4,229384
-pyaon.pyi,sha256=nW67oWMxc6ky4xTpgPFC0BcpLhxx8ryGaNVBXh_ySgo,191
-pyaon-1.1.6.dist-info/top_level.txt,sha256=LPUN0efVsztG5cB2qwCc72OHMn3GFT4Ti6ZzEvSws2M,6
-pyaon-1.1.6.dist-info/LICENSE-3RD-PARTY,sha256=g5ZbhDuY9nDTqFvQQe1LNyyOxQ17SlmVqDrGl7pnXcs,1684
-pyaon-1.1.6.dist-info/RECORD,,
-pyaon-1.1.6.dist-info/WHEEL,sha256=aIHtXq4XssUHqceM9ZWc7TXyJq4AMH0BhNTZQBcVTZY,162
-pyaon-1.1.6.dist-info/METADATA,sha256=wpYn44QQIgNTeUcUrZ4iWbFTPcTwp959bv91-SSdUiA,1746
+pyaon.pypy39-pp73-x86_64-linux-gnu.so,sha256=esdx9b9K766GA7WTiRsg77bvKIprLD-t8J_jbxhG4hk,229384
+pyaon.pyi,sha256=z_3k3wd_KIK6Sb4ltnGNYzYkAE-Ht-P3DDuPQ5ZeRac,204
+pyaon-1.1.7.dist-info/top_level.txt,sha256=LPUN0efVsztG5cB2qwCc72OHMn3GFT4Ti6ZzEvSws2M,6
+pyaon-1.1.7.dist-info/LICENSE-3RD-PARTY,sha256=g5ZbhDuY9nDTqFvQQe1LNyyOxQ17SlmVqDrGl7pnXcs,1684
+pyaon-1.1.7.dist-info/RECORD,,
+pyaon-1.1.7.dist-info/WHEEL,sha256=aIHtXq4XssUHqceM9ZWc7TXyJq4AMH0BhNTZQBcVTZY,162
+pyaon-1.1.7.dist-info/METADATA,sha256=rh1kCzpHJbPeTUax3z5LXsBEEHdD8FdC9pYBYvtX-zM,1746
```

## Comparing `pyaon-1.1.6.dist-info/METADATA` & `pyaon-1.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaon
-Version: 1.1.6
+Version: 1.1.7
 Summary: python bindings for the aon library
 Home-page: https://github.com/Tomcat-42/pyaon
 Author: Pablo Alessandro Santos Hugen
 Author-email: pablohuggem@gmail.com
 License: Public Domain
 Keywords: text file format serialization deserialization binary data compression
 Classifier: Development Status :: 4 - Beta
```


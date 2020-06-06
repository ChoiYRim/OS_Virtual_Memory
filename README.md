# OS_Virtual_Memory

[CAUTION]

If you want to execute this source code on your computer, you have to run this software on 32bit Ubuntu Linux 16.04. In addition, The size of physical memory of the 'SSUOS' which is OS for practice is 128MB and the size of one page frame is 4KB.

I'm not a native English speaker,so please consider it when you read this script. :)

[COPYRIGHT]

All copyright is belong to Soongsil University OS Lab and this project was sixth subject of OS class.

[OVERVIEW]

The main object of this project is to make a 'Page Allocator'. To make this project, We need to understand what the virtual 
memory is and what the paging is. Virtual memory is to offer much bigger address space than real existing memory space by 
abstracting physical memory. This address space is called 'Page' that points 4KB memory pieace. If we know the definitions of 
the virtual memory and the paging, we can understand that it is impossible to match one to one between virtual memory and 
physical memory.

The object of this project is to make 'Page Allocator' based on understanding of virtual memory space and paging method. The virtual memory is splited into 'Kernel Pool' and 'User Pool' that we have to manage an usable page frame by bitmap. The main
aims were written at [OBJECTS].

If you want to execute this source code on your computer, you have to run this software on 32bit Ubuntu Linux 16.04. In 
addition, The size of physical memory of the 'SSUOS' which is OS for practice is 128MB and the size of one page frame is 4KB.


[OBJECTS]

1. Make kernel pool and user pool : I wrote them in 'init_palloc()' of palloc.c

2. Make memory allocating function and deleting function in palloc.c : 
   -> 'palloc_get_multiple_page()' and 'palloc_free_multiple_page()'

3. Make page directory and page table when the process is made : 'pd_create()','pd_copy()',and 'pt_copy()' of paging.c

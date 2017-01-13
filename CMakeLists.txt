message(STATUS "Entering directory .")
cmake_minimum_required(VERSION 3.1.0 FATAL_ERROR)
project(vlink C)

set(vlink_SRCS
    main.c        
    support.c     
    errors.c      
    linker.c      
    dir.c         
    targets.c     
    ar.c          
    pmatch.c      
    ldscript.c    
    expr.c        
    t_amigahunk.c 
    elf.c         
    t_elf32.c     
    t_elf32ppcbe.c
    t_elf32m68k.c 
    t_elf32jag.c  
    t_elf32i386.c 
    t_elf32arm.c  
    t_elf64.c     
    t_elf64x86.c  
    t_aout.c      
    t_aoutnull.c  
    t_aoutm68k.c  
    t_aouti386.c  
    t_aoutmint.c  
    t_ataritos.c  
    t_rawbin.c    
    t_rawseg.c    
    t_vobj.c)

add_executable(vlink ${vlink_SRCS})

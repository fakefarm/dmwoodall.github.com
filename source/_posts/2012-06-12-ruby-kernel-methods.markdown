---
layout: post
title: "ruby kernel methods"
date: 2012-06-12 19:16
comments: true
categories: 
published: false
---

ruby -e 'print Kernel.private_instance_methods(false).sort'

:Array 
:Complex,
:Float, 
:Integer, 
:Rational, 
:String, 
:__callee__, 
:__method__, 
:`
:abort
:at_exit
:autoload, :autoload?, :binding, :block_given?, :caller, :catch, :eval, :exec, :exit, :exit!, :fail, :fork, :format, :gem, :gem_original_require, :gets, :global_variables, :initialize_copy, :iterator?, :lambda, :load, :local_variables, :loop, :open, :p, :print, :printf, :proc, :putc, :puts, :raise, :rand, :readline, :readlines, :remove_instance_variable, :require, :require_relative, :select, :set_trace_func, :sleep, :spawn, :sprintf, :srand, :syscall, :system, :test, :throw, :trace_var, :trap, :untrace_var, :warn
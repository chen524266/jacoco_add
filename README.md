###Introduction

Based on the jacoco branch  0.8.7, generate incremental code coverage and merge different exec files at different classId and different time.

Please refer to the blog for the second development strategy https://blog.csdn.net/qq_34418450/article/details/135386280?spm=1001.2014.3001.5501

I won't go into detail here.

Usage:

--Diffcode is incremental statistics, without it, the total quantity is counted.

--OnlyMergeExec=true Do not generate reports, merge probe data, and generate merged exec files

--MergeExecfilepath requires merging exec probe files

--MergeClassfilepath: The path to the class file that needs to be merged

--MergeExec specifies the path to generate a new exec file after merging probe data

Example of merging probe data to generate exec:

File HTML=new File ("D: \ \ home");

Execute ("report", "D: \ \ jacoco_merge_test. exec", "-- classfiles",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ bbzx \ \ com",

"-- classfiles",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ common \ \ com",

"-- classfiles",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ reportsupport \ \ com",

"-- classfiles",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ reportview \ \ com",

"-- classfiles",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ website \ \ com",

"-- mergeExecfilepath",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616785_616788 \ \ execfiles \ \ jacoco20240109165235. exec",

"-- mergeClassfilepath",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ bbzx \ \ com",

"-- mergeClassfilepath",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ reportview \ \ com",

"-- mergeClassfilepath",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ common \ \ com",

"-- mergeClassfilepath",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ reportsupport \ \ com",

"-- mergeClassfilepath",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ classfiles \ \ website \ \ com",

"-- sourcefiles",

"D: \ \ gitworkplace \ \ luckframeweb \ \ coverage \ \ trunk \ \ 616788 \ \ sourcefiles",

"-- onlyMergeExec", "true",

"-- mergeExec", "D: \ \ jacoco_merge_test. exec",

"-- HTML", HTML. getAbsolutePath();
 
 

### 简介
   基于ray大佬的分支二开，感谢大佬的无私奉献。jacoco二开，增量覆盖率和不同时间节点的不同class代码覆盖率合并功能。
 二开思路请参考博文https://blog.csdn.net/qq_34418450/article/details/135386280?spm=1001.2014.3001.5501
 这里不再赘述。
 使用方法:
 --diffcode是增量统计，不带则统计全量。
 --onlyMergeExec=true 不生产报告，合并探针数据，生成合并后的exec文件
 --mergeExecfilepath 需要合并的exec探针文件
 --mergeClassfilepath 需要合并的class文件路径
 --mergeExec 指定探针数据合并后生成新的exec文件路径
 合并探针数据生成exec的例子:
 	File html = new File("D:\\home");
		execute("report", "D:\\jacoco_merge_test.exec", "--classfiles",
				"D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\bbzx\\com",
				"--classfiles",
				"D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\common\\com",
				"--classfiles",
				"D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\reportsupport\\com",
				"--classfiles",
				"D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\reportview\\com",
				"--classfiles",
				"D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\website\\com",
				 "--mergeExecfilepath",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616785_616788\\execfiles\\jacoco20240109165235.exec",
				 "--mergeClassfilepath",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\bbzx\\com",
				 "--mergeClassfilepath",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\reportview\\com",
				 "--mergeClassfilepath",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\common\\com",
				 "--mergeClassfilepath",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\reportsupport\\com",
				 "--mergeClassfilepath",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\classfiles\\website\\com",
				 "--sourcefiles",
				 "D:\\gitworkplace\\luckframeweb\\coverage\\trunk\\616788\\sourcefiles",
				 "--onlyMergeExec", "true",
				 "--mergeExec", "D:\\jacoco_merge_test.exec",
				"--html", html.getAbsolutePath());
 
 ###Introduction

Based on the branch of Ray Big Boss, thank you for your selfless dedication. Jacoco two open, merging incremental coverage and different class code coverage at different time nodes.

Please refer to the blog for the second development strategy https://blog.csdn.net/qq_34418450/article/details/135386280?spm=1001.2014.3001.5501

I won't go into detail here.

Usage:

--Diffcode is incremental statistics, without it, the total quantity is counted.

--OnlyMergeExec=true Do not produce reports, merge probe data, and generate merged exec files

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
 
 

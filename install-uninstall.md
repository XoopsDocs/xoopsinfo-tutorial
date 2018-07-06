# Install/Uninstall

## Introduction

**XoopsInfo** is an administration module that provides a bit of useful administrative information to your fingertips. Every site should have access to this information. It also has a rescue capability.

XoopsInfo Provides the following information:

* Basic XOOPS setting info of high import -- all accessible in other locations
* PHP Server Info -- one could easily make this available as it's just the phpinfo\(\) function
* MySQL Info - basic settings as well as access to some management controls of tables \(setup in the module prefs\)
* Module Info - a better formatted version of the system administration modules page along with some useful links
* WYSIWYG Editor info on installed \(but not versions\)
* Template overriding from themes directories
* System Info \(phpSysInfo\)
* PHP Security Info \(phpSecInfo\)

There are several parts to the package:

* the module
* two supporting apps - phpsecinfo and phpsysinfo
* mimetype manager update - modifies core files, so may not want to install

XoopsInfo generally works fine with just the module. However, you may get additional desired functionality using the extra files, but you will have to make sure core updates don't overwrite them and/or merge updates\).

## 1.0 Install/Uninstall

No special measures necessary, follow the standard installation process � extract the module folder into the

/modules

directory in your XOOPS installation. Install the module through Admin -&gt; System Module -&gt; Modules.

Detailed instructions on installing modules are available in the [**Chapter 2.12 of our XOOPS Operations Manual**](https://www.gitbook.com/book/xoops/xoops-operations-guide/)

Install/Upgrade the module normally. Then download phpsecinfo and phpsysinfo. By default, these are stored in xoopsinfo/phpsecinfo and xoopsinfo/phpsysinfo, but you may place them wherever you'd like, including the xoops\_trusted\_path \(which helps prevent them from being run by other people\). If desired, install the mimetype manager update. Configurations

There is a rescue capability, but you must specify a password in configuration for it to work. Path is:

```text
XOOPS_ROOT/modules/xoopsinfo/admin/rescue.php.
```

You may want to modify the referrers so you can access certain aspects of the module.

You may want to change the language \(and theme\) for phpsysinfo \(I hope it tries to call the XOOPS language first, but don't know\).


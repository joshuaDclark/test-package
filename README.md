## A simple Composer test package.


### This is a little composer package I made to better understand how I could expedite my future projects. The idea is for this to behave as a starter kit for my project's scaffolding. 


This doc will show you how to set this up in 2 minutes or less.


If you prefer a video tutorial you can watch this [here](https://www.loom.com/share/a1bbfe71aa7c4915b1837eaff0a4d8c0?sid=0d326905-c632-4e52-8a0a-b4cc7864b802).

---

Requirements:
- PHP must be installed (latest version is ideal)
- Latest version of Composer must be installed


1. Start a new project.
2. In your root directory add a composer.json file and copy the following snippet of code:

```
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/joshuaDclark/test-package"
    }
  ],
  "require": {
    "jc/test": "dev-master"
  }
}
```

3. Run `composer install`

4. Create a file called `test.php` and add the following snippet

```
    <?php

    require_once 'vendor/autoload.php';

    sayHello();

```

Save to the project root directory.


5. Run the following command:

   `php test.php`

After running this command you should see the following response:

`Hello from my test package! This is from V-2`

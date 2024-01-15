## A simple Composer test package.


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

```<?php

    require_once 'vendor/autoload.php

    sayHello();
```

Save to the project root directory.


5. Run the following command:

   `php test.php`

After running this command you should see the following response:

`Hello from my test package! This is from V-2`

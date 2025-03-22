# LKS Cloud Computing DIY 2024

Repository ini merupakan aplikasi berbasis web yang digunakan untuk seleksi LKS DIY 2024 bidang Cloud Computing.

```
‌‌         ∩∩   ♡      i will always be
       (  . .̫ . )     here for supporting
 〃 ∩    ◜◝U-U◜◝       and loving you lkscc..
 ⊂   ⌒ (   。・ ㉨ ・  )
    ヽ  _ つ＿/￣￣￣/
　 　     ＼/＿＿＿/
```

## Requirements
 - [v8.1+](https://www.php.net/)
 - [Composer v2](https://yarnpkg.com/en/docs/install)
## Getting started
### Clone the repo:
```bash
git clone --depth 1 https://github.com/therusetiawan/lksdiycc2024
cd lksdiycc2024
rm -rf .git
```

### Set environment variables:
```bash
cp .env.example .env
```

### Install dependencies:
```bash
composer update
```

### Set key:
```bash
php artisan key:generate
```

### Set database on .env (fill your AWS database config):
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=
```

### Set S3 on .env (fill your AWS S3 config):
```bash
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_DEFAULT_REGION=ap-southeast-2
AWS_BUCKET=
AWS_USE_PATH_STYLE_ENDPOINT=false
```

### Set Redis ElastiCache on .env (fill your AWS ElasticCache config):
```bash
REDIS_HOST=127.0.0.1
REDIS_PASSWORD=null
REDIS_PORT=6379
```

### Database migration and seed:
```bash
php artisan migrate
```

### Running locally (in personal computer):
```bash
php -S localhost:8000 -t public
```

## License and Copyright

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

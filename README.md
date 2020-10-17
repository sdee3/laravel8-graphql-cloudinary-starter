<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Contents

This project consists of the following packages I additionaly set-up:
- [GraphQL](https://lighthouse-php.com/) (with MySQL, a complete switch to [MongoDB](https://github.com/jenssegers/laravel-mongodb) is being discussed in my head)
- ESLint ([huge thanks to Wesbos for his template](https://github.com/wesbos/eslint-config-wesbos))
- [Cloudinary API](https://github.com/cloudinary-labs/cloudinary-laravel)

### Post-Installation Set-up, AKA How to make above mentioned packages working
* `php artisan vendor:publish --tag=lighthouse-schema`
* `npx install-peerdeps --dev eslint-config-wesbos`
* `php artisan vendor:publish --provider="CloudinaryLabs\CloudinaryLaravel\CloudinaryServiceProvider" --tag="cloudinary-laravel-migration"`
* `php artisan vendor:publish --provider="CloudinaryLabs\CloudinaryLaravel\CloudinaryServiceProvider" --tag="cloudinary-laravel-config"`

Or follow the guides for each package, I might have pasted unnecessary lines 😊

If you're going to use Cloudinary API, don't forget to set the `CLOUDINARY_URL` key in your `.env` file.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

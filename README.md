# GhasedakSms-Iran

1. composer require Alirezamosavi/GhasedakSms-Iran

2. php artisan vendor:publish --tag=config

3. add the below code in .env
GHASEDAK_API_KEY="${GHASEDAK_API_KEY}"
GHASEDAK_LINE_NUMBER="${GHASEDAK_LINE_NUMBER}"
GHASEDAK_LINE_NUMBERS="${GHASEDAK_LINE_NUMBERS}"

4. add the below code in route/web.php
Route::get('/', function () {

    $sms = GhasedakSms::sendSingleSMS('alirezacvvv', '09138726138');
    //return view('welcome');
});

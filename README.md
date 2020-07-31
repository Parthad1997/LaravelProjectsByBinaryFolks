# LaravelProjectsByBinaryFolks

//web.php

Route::get('/','SiteController@Home');

Route::get('/','SiteController@About');


Route::get('/','SiteController@Contact');


# view

# HomePAge.blade.php
<h1> This is Home Page </h1>

# AboutPage.blade.php
<h1> This is Home Page </h1>

# ContactPage.blade.php
<h1> This is Home Page </h1>

# SiteController.php

namespace App\Http\Controllers;

use Illuminate\Foundation\Auth\Access\AuthorizesRequests;
use Illuminate\Foundation\Bus\DispatchesJobs;
use Illuminate\Foundation\Validation\ValidatesRequests;
use Illuminate\Routing\Controller as BaseController;

class SiteController extends Controller
{
    function Home()
    {
    	return view('HomePage');
	
    }
        function About()
    {
    	return view('AboutPage');
	
    }
        function Contact()
    {
    	return view('ContactPage');
	
    }
}







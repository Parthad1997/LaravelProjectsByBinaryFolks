# LaravelProjectsByBinaryFolks

Route::get('/posts/{post}',function($post))
{
	$posts=[
		'First post'=>'Hello';
		'Second post'=>'New i am getting';

		if(! array_key_exists($post, $posts)){
			abort(404,'Sorry wrong req');

		}
		return view('post';['post'=>$posts[$post]]);
	})
		}
	]
}

# Teorihandboken - Programmeringsmetodik (PG)
Studerande: Förnamn Efternamn

## PG 1.1 Versionshantering (Git)
Beskriv rubriken här

## PG 1.2 Benchmarking
Beskriv rubriken här

## PG 1.3 Testdriven utveckling
Beskriv rubriken här

## PG 1.4 Deploy och staging
Beskriv rubriken här

## PG 1.5 Debugging
Beskriv rubriken här

## PG 1.6 Dokumentation
Beskriv rubriken här

## PG 1.7 Struktur av kod i projekt

Det är super viktigt att skriva kod som är lätt att läsa och fixa om det behövs. Inte bara för mig själv, utan även om det är flera som jobbar på ett projekt. Då måste alla hålla sig till samma sätt att skriva kod så att alla förstår hur allting funkar. Oftast använder man en slags guide för hur man ska skriva koden, som säger hur den ska se ut, vad variabler och funktioner ska heta, och så vidare.

Ett bra exempel från vårt tidigare projekt, U05AN, var att vi hade en bra struktur på koden, så det var enkelt för alla att hitta sin egen kod. Här nedan kan du se hur vi strukturerade våra routes på ett väldigt smidigt och enkelt sätt för att undvika att oavsiktligt ändra någon annans route.

// Daniel
// comments 
// Route::get('/comment', [CommentController::class, 'index'])->name('comments.index');
// Route::post('/comment', [CommentController::class, 'store'])->name('comments.store');
// Route::get('/movies/{id}', [CommentController::class, 'show'])->name('movies.show');
// Route::post('/movies/{id}/comment', [CommentController::class, 'store'])->name('movies.comment');
// Route::get("/comment/{movie_id}", [CommentController::class, 'getCommentsByMovies'])->name('comments.movie');
// Route::get('/comments', [CommentController::class, 'allMoviesComments'])->name('comments');


//Lolo

//MyList:
// Route::get('/mylist', [MyListController::class, 'show'])->name('mylist.show');

// Route::get('/mylist/delete/{movie_id}', [MyListController::class, 'deleteMovie']);

//check the user that logged in, get their mylist with user id and then just detach the movie id from the pivot table


// Route::get('/mylist', [MyListController::class, 'show'])->name('mylist.show');
// Route::get('/mylist/{movie_id}', [MyListController::class, 'addMovie'])->name('mylist.add');


// Mohamed Abdi
// Update country movies

// Route::get('/country', [CountryController::class, 'index'])->name('country.index');
// Route::get('/country/filter', [CountryController::class, 'filter'])->name('country.filter');



// mohamed adbi 
// genre update 



// Define your routes
// Route::get('/genre', [GenreController::class, 'index'])->name('genre.index');
// Route::get('/genre/filter', [GenreController::class, 'filter'])->name('genre.filter');
// Route::post('/movies/{movie}/comment', [GenreController::class, 'comment'])->name('movies.comment');

--------------------------------------------------------------------------------------------------------------------------
En annan viktig del inom struktur av kod i ett projekt är att man kommenterar sin kod. När jag skriver kod är det viktigt för mig att lägga till kommentarer. Det hjälper mig själv och andra att förstå vad varje del av koden gör. Kommentarerna fungerar som små förklaringar som berättar vad varje bit kod gör och varför den är viktig. På så sätt kan jag och andra lättare följa min tankegång och förstå koden bättre. Dessutom kan kommentarerna ge tips och förklaringar om eventuella problem eller särskilda saker att tänka på. Så när jag inkluderar tydliga kommentarer i min kod gör jag den mer användbar och lättare att förstå och jobba med. 


## PG 1.8 Automatisering av arbetsflöde
Beskriv rubriken här

## PG 1.9 Virtualisering av utvecklingsmiljö
Beskriv rubriken här

## PG 1.10 Bundeling-verktyg
Beskriv rubriken här

## PG 1.11 Terminalinterface
Beskriv rubriken här


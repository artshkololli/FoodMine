#Steps\
&emsp;1.Install dev tools\
&emsp;2.Create Angular App\
&emsp;3.Create project folder\
&emsp;4.Install @angular/cli\
&emsp;5.Create Frontend folder\
&emsp;&emsp;5.1.Add Header\
&emsp;&emsp;&emsp;&emsp;5.1.1.Create Header Component\
&emsp;&emsp;&emsp;&emsp;5.1.2.Add HTML/CSS\
&emsp;&emsp;5.2.List Foods\
&emsp;&emsp;&emsp;&emsp;5.2.1.Create Food model\
&emsp;&emsp;&emsp;&emsp;5.2.2.Create data.ts\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.2.2.1.Add sample data\
&emsp;&emsp;&emsp;&emsp;5.2.3.Add images to assets\
&emsp;&emsp;&emsp;&emsp;5.2.4.Create Food service\
&emsp;&emsp;&emsp;&emsp;5.2.5.Create Home Component\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.2.5.1.Add HTML/CSS/TS\
&emsp;&emsp;5.3.Add Search Feature\
&emsp;&emsp;&emsp;&emsp;5.3.1.Add method(service)\
&emsp;&emsp;&emsp;&emsp;5.3.2.Add search route(app-routing,router-outlet tag in app component)\
&emsp;&emsp;&emsp;&emsp;5.3.3.Show search result in Home Component(activatedRoute in constructor)\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.3.1.Use activatedRoute.params.subscribe() to get result\
&emsp;&emsp;&emsp;&emsp;5.3.4.Create Search Component\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.1.Add to Home Component\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.Add HTML/CSS/TS\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.1.Add empty search variable\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.2.Add activatedRoute in constructor\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.3.Add private router:Router in constructor\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.4.Use activatedRoute.params.subscribe() to get result\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.5.Create searchBar function(navigateByUrl)\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.6.Add input tag(#s reference template)\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.7.Add to input tag (keyup.enter)="Searchbar(s.value)"\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.8.Add to input tag [value]="search"\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.9.Add button tag(click="searchBar(s.value)")\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.3.4.2.10.Add CSS\
&emsp;&emsp;5.4.Add Tag Bar\
&emsp;&emsp;&emsp;&emsp;5.4.1.Create Tag Model(models folder)\
&emsp;&emsp;&emsp;&emsp;5.4.2.Add sample tags to data.ts\
&emsp;&emsp;&emsp;&emsp;5.4.3.Add Food tags service (food.service.ts file)\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.3.1.Add get all tags method\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.3.2.Add get all foods by tag method\
&emsp;&emsp;&emsp;&emsp;5.4.4.Add tags route(app-routing)\
&emsp;&emsp;&emsp;&emsp;5.4.5.Show tag result in Home Component(add else if to activatedRoute.params.subscribe)\
&emsp;&emsp;&emsp;&emsp;5.4.6.Create Tags Component\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.1.Add to Home Component(app-tags html tag)\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.2.Add HTML/CSS/TS\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.2.1.Add empty tag array variable\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.2.2.Add foodService in constructor and get all tags\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.2.3.Add div *ngIf="tags" directive\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.2.4.Add html tag a with *ngFor and routerLink directives\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.4.6.2.5.Add CSS\
&emsp;&emsp;5.5.Add Food Page\
&emsp;&emsp;&emsp;&emsp;5.5.1.Add method to food service(use .find)\
&emsp;&emsp;&emsp;&emsp;5.5.2.Create Food Page Component\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.5.2.1.Add food page route(app-routing, component:FoodPageComponent)\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.5.2.2.Add empty food variable of type Food\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.5.2.3.Add activatedRoute and foodService in constuctor\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.5.2.4.Use activatedRoute.params.subscribe()\
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;5.5.2.5.Add HTML/CSS (use *ngFor to show origins and tags (add routerLink))\
&emsp;&emsp;5.6.Add Cart Page\
&emsp;&emsp;&emsp;&emsp;5.6.1.Create Cart and CartItem Models\
&emsp;&emsp;&emsp;&emsp;5.6.2.Add Cart service(ng g s services/cart in terminal)\
&emsp;&emsp;&emsp;&emsp;5.6.3.Create private cart:Cart=new Cart(Changed to this.getCartFromLocalStorage() later)\
&emsp;&emsp;&emsp;&emsp;5.6.4.Create private cartSubject:BehaviorSubject<Cart>=new BehaviorSubject(this.cart)\
&emsp;&emsp;&emsp;&emsp;5.6.5.Import BehaviorSubject from rxjs\
&emsp;&emsp;&emsp;&emsp;5.6.6.Add addToCart Method (use .find() and .push())\
&emsp;&emsp;&emsp;&emsp;5.6.7.Add removeFromCart Method (use .filter())\
&emsp;&emsp;&emsp;&emsp;5.6.8.Add clearCart and changeQuantity Method (use .find())\
&emsp;&emsp;&emsp;&emsp;5.6.9.Add getCartObservable Method (return this.carSubject.asObservable())\
&emsp;&emsp;&emsp;&emsp;5.6.10.Import Observable from rxjs\
&emsp;&emsp;&emsp;&emsp;5.6.11.Add private setCartToLocalStorage():void method\
&emsp;&emsp;&emsp;&emsp;5.6.12.Get totalPrice and totalCount using .reduce() method\
&emsp;&emsp;&emsp;&emsp;5.6.13.Use JSON.Stringify on this.cart to set the Cart to localStorage\
&emsp;&emsp;&emsp;&emsp;5.6.14.Use this.cartSubject.next(this.cart)\
&emsp;&emsp;&emsp;&emsp;5.6.15.Add private getCartFromLocalStorage():Cart method\
&emsp;&emsp;&emsp;&emsp;5.6.16.Use setCartToLocalStorage method on all methods except getCartObservable()\
&emsp;&emsp;&emsp;&emsp;5.6.17.Add private cartService:CartService and router:Router to Food Page constructor\
&emsp;&emsp;&emsp;&emsp;5.6.18.Add addToCart method in Food Page\
&emsp;&emsp;&emsp;&emsp;5.6.19.Add addToCart method to the button in Food Page Component\
&emsp;&emsp;&emsp;&emsp;5.6.20.Create cart-page Component\
&emsp;&emsp;&emsp;&emsp;5.6.21.Add Route for cart-page(app-routing)\
&emsp;&emsp;&emsp;&emsp;5.6.22.Add private cartService in cart-page constructor and use .subscribe method\
&emsp;&emsp;&emsp;&emsp;5.6.23.Add removeFromCart and changeQuantity methods\
&emsp;&emsp;&emsp;&emsp;5.6.24.Create title Component in partials folder\
&emsp;&emsp;&emsp;&emsp;5.6.25.Add app-title to cart-page\
&emsp;&emsp;&emsp;&emsp;5.6.26.Add @Input to title component(title! , margin? , fontSize? inputs)\
&emsp;&emsp;&emsp;&emsp;5.6.27.Use inputs in title component html(use [ngStyle] for margin and fontsize)\
&emsp;&emsp;&emsp;&emsp;5.6.28.Add CSS to title component\
&emsp;&emsp;&emsp;&emsp;5.6.29.Show cartItems in cart page\
&emsp;&emsp;&emsp;&emsp;5.6.30.Use select tag for quantity selection(use #quantitySelect on tag)\
&emsp;&emsp;&emsp;&emsp;5.6.31.Show price of cartItems\
&emsp;&emsp;&emsp;&emsp;5.6.32.Add Remove button\
&emsp;&emsp;&emsp;&emsp;5.6.33.Add Checkout with totalCount and totalPrice in cart page\
&emsp;&emsp;&emsp;&emsp;5.6.34.Add CSS\
&emsp;&emsp;&emsp;&emsp;5.6.35.Add cartService to header constuctor and show quantity in header component\
&emsp;&emsp;5.7.Add Not Found Page\
&emsp;&emsp;&emsp;&emsp;5.7.1.Create not-found Component\
&emsp;&emsp;&emsp;&emsp;5.7.2.Add app-not-found to cart-page component\
&emsp;&emsp;&emsp;&emsp;5.7.3.Add visible,notFoundMessage,resetLinkText,resetLinkRoute @Input in not-found class\
&emsp;&emsp;&emsp;&emsp;5.7.4.Add @input in cart-page component (inside app-not-found)\
&emsp;&emsp;&emsp;&emsp;5.7.5.Add CSS\
&emsp;&emsp;&emsp;&emsp;5.7.6.Add app-not-found to all pages\
&emsp;6.Create Backend folder\
&emsp;&emsp;6.1.Use npm init -y in terminal and install Typescript\
&emsp;&emsp;6.2.Create a tsconfig.json file\
&emsp;&emsp;6.3.Create src folder and .gitignore file\
&emsp;&emsp;6.4.Copy data.ts to backend/src(change array names to any)\
&emsp;&emsp;6.5.Install express cors\
&emsp;&emsp;6.6.Create server.ts file\
&emsp;&emsp;&emsp;&emsp;6.6.1.Install types@express and import express in server.ts file\
&emsp;&emsp;&emsp;&emsp;6.6.2.Install types@cors and import cors in server.ts file\
&emsp;&emsp;&emsp;&emsp;6.8.3.Create express application(app=express()), use app.use,app.get,app.listen\
&emsp;&emsp;&emsp;&emsp;6.8.4.Install ts-node and nodemon(use --save-dev for both)\
&emsp;&emsp;&emsp;&emsp;6.8.5.Add a start script in package.json(value of start is "cd src && nodemon server.ts")\
&emsp;&emsp;&emsp;&emsp;6.8.5.Make api requests for sample_foods,searchTerm,tags,tagName,foodId\
&emsp;&emsp;6.7.Create constants folder in shared folder in frontend,create urls.ts\
&emsp;&emsp;&emsp;&emsp;6.7.1.add BASE_URL="backend url",FOODS,FOODS_TAGS,FOOD_BY_SEARCH,FOODS_BY_ID(add _URL)\
&emsp;&emsp;6.8.Add HttpClient Module(import in app.module.ts)\
&emsp;&emsp;&emsp;&emsp;6.8.1.Inject HttpClient in food.service constructor(private http)\
&emsp;&emsp;&emsp;&emsp;6.8.2.Use Observable for methods(<Food[]>,<Tag[]>,<Food>)\
&emsp;&emsp;6.9.Add let foodsObservable:Observable<Food[]> in home component constructor(replace this.foods)\
&emsp;&emsp;6.10.Use .subscribe() at the end of else statement\
&emsp;&emsp;6.11.For food-page and tags components remove this.foods and subscribe to the method\
&emsp;&emsp;6.12.Change food.id to just food in food page html file\
&emsp;&emsp;6.13.Adding Login\
&emsp;&emsp;&emsp;&emsp;6.13.1.Create login-page Component\
&emsp;&emsp;&emsp;&emsp;6.13.2.Add component to route(app-routing)\
&emsp;&emsp;&emsp;&emsp;6.13.3.Import FormGroup,FormBuilder,Validators from @angular/forms\
&emsp;&emsp;&emsp;&emsp;6.13.4.Add a loginForm of type FormGroup , add private formBuilder in constructor\
&emsp;&emsp;&emsp;&emsp;6.13.5.Use Validators on loginForm inside ngOnInit method\
&emsp;&emsp;&emsp;&emsp;6.13.6.Add email and password controls for loginForm(use formBuilder.group())\
&emsp;&emsp;&emsp;&emsp;6.13.7.Make a get fc() method that returns this.loginForm.controls(fc=form control)\
&emsp;&emsp;&emsp;&emsp;6.13.8.Create submit() method to check if form is invalid and to check form values\
&emsp;&emsp;&emsp;&emsp;6.13.9.Add ReactiveFormsModule to app.module imports\
&emsp;&emsp;&emsp;&emsp;6.13.10.Add a form in login-page (use [formGroup] and (ngSubmit))\
&emsp;&emsp;&emsp;&emsp;6.13.11.Add an "error-list" div and show when input is invalid for email and password\
&emsp;&emsp;&emsp;&emsp;6.13.12.Use *ngIf to check if email and password is valid , show message if its not\
&emsp;&emsp;&emsp;&emsp;6.13.13.Add Login API\
&emsp;&emsp;&emsp;&emsp;6.13.14.Add app.post("api/users/login) method in backend server\
&emsp;&emsp;&emsp;&emsp;6.13.15.Add app.use(express.json) to allow requests with json body on API\
&emsp;&emsp;&emsp;&emsp;6.13.16.Add sample_users in data.ts\
&emsp;&emsp;&emsp;&emsp;6.13.17.Use .find() method to find user in app.post() , if user exist send request\
&emsp;&emsp;&emsp;&emsp;6.13.18.Install jsonwebtoken(JWT) library and @types/jsonwebtoken to generate tokens\
&emsp;&emsp;&emsp;&emsp;6.13.19.Create generateTokenResponse=(user:any) const (use jwt.sign())\
&emsp;&emsp;&emsp;&emsp;6.13.20.Try POST request with Postman\
&emsp;&emsp;6.14.Create User Service\
&emsp;&emsp;&emsp;&emsp;6.14.1.Create User model (shared/models folder)\
&emsp;&emsp;&emsp;&emsp;6.14.2.Create private userSubject=BehaviourSubject<User>(new User())\
&emsp;&emsp;&emsp;&emsp;6.14.3.Create public userObservable=:Observable<User>\
&emsp;&emsp;&emsp;&emsp;6.14.4.Initialize this.userObservable=this.userSubject.asObservable() in constructor\
&emsp;&emsp;&emsp;&emsp;6.14.5.Create interfaces folder in shared folder and make a IUserLogin.ts file\
&emsp;&emsp;&emsp;&emsp;6.14.6.Create login(userLogin:IUserLogin):Observable<User> method and make post request\
&emsp;&emsp;&emsp;&emsp;6.14.7.Add private http:HttpClient in constructor\
&emsp;&emsp;&emsp;&emsp;6.14.8.Add USER_LOGIN_URL to urls.ts file\
&emsp;&emsp;&emsp;&emsp;6.14.9.Use .pipe(tap()) method on login post request\
&emsp;&emsp;&emsp;&emsp;6.14.10.Install ngx-toastr module\
&emsp;&emsp;&emsp;&emsp;6.14.11.Install ngx-toastr module , import ToastrModule and BrowserAnimation (app.module)\
&emsp;&emsp;&emsp;&emsp;6.14.12.Import ToastrModule.forRoot({timeOut,positionClass,newestOnTop}) in imports:[]\
&emsp;&emsp;&emsp;&emsp;6.14.13.Add private toastrService:ToastrService , use toastrService.success in login()\
&emsp;&emsp;&emsp;&emsp;6.14.14.Add "node_modules/ngx-toastr/toastr.css" to styles in angular.json file\
&emsp;&emsp;&emsp;&emsp;6.14.15.Add private userService:UserService in login-page constructor, use it in submit()\
&emsp;&emsp;&emsp;&emsp;6.14.16.Add private activatedRoute:ActivatedRoute,private router:Route same constructor\
&emsp;&emsp;&emsp;&emsp;6.14.17.Add this.returnUrl=this.activatedRoute.snapshot.queryParams.returnUrl to ngOnInit\
&emsp;&emsp;&emsp;&emsp;6.14.18.Create private setUserToLocalStorage(user:User) method on user.service\
&emsp;&emsp;&emsp;&emsp;6.14.19.Create private getUserFromLocalStorage():User method on user.service\
&emsp;&emsp;&emsp;&emsp;6.14.20.Add const USER_KEY='User' in user.service(between imports and @injectable)\
&emsp;&emsp;&emsp;&emsp;6.14.21.Change new User() to this.getUserFromLocalStorage() in private userSubject\
&emsp;&emsp;&emsp;&emsp;6.14.22.Add private userService in header component constructor , add user!:User variable\
&emsp;&emsp;&emsp;&emsp;6.14.23.Put {{user.name}} in <a routerLink="/dashboard"> at header component html\
&emsp;&emsp;&emsp;&emsp;6.14.23.Create isAuth() that returns this.user.token\
&emsp;&emsp;&emsp;&emsp;6.14.23.Add *ngIf="!isAuth" to first <li>tag in header component\
&emsp;&emsp;&emsp;&emsp;6.14.23.Create logout method in user.service\
&emsp;&emsp;&emsp;&emsp;6.14.23.Create logout method in header component.ts\
&emsp;&emsp;&emsp;&emsp;6.14.23.Add logout method to lougout link (a tag) add *ngIf="isAuth" to that li tag\






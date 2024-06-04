# flutter-japanese-restaurant-app

Japanese restaurant app is a design implementation of [Japanese restaurant app](https://dribbble.com/shots/14752424-Japan-Restaurant-App-Food-App/attachments/6455673?mode=media)
![](screenshots/japanese_restaurant_app_dark.png?raw=true)
![](screenshots/japanese_restaurant_app_light.png?raw=true)



## Screenshots (Light mode)

Preview                    |   Home screen             |  Food Detail Screen    |  Cart Screen
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
![](screenshots/preview.gif?raw=true)|![](screenshots/food_list_screen_light.png?raw=true)|![](screenshots/food_detail_screen_light.png?raw=true)|![](screenshots/cart_screen_light.png?raw=true)

## Screenshots (Dark mode)

Favorite screen            |   Home screen             |  Food Detail Screen       |  Cart Screen
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
![](screenshots/favorite_screen_dark.png?raw=true)|![](screenshots/food_list_screen_dark.png?raw=true)|![](screenshots/food_detail_screen_dark.png?raw=true)|![](screenshots/cart_screen_dark.png?raw=true)


## 🚀 Features :
```
• Dynamically change between light and dark theme
• Bottom navigation animation when switch from one screen to another
• Fade animation for food items in detail screen and list views
• Delete single food item from cart by swipe item to right side
• Automatically delete single item from cart by set its value to zero
• Increase or Decrease quantity for each food item in cart screen
• Display food list on the food list screen
• Display Detail of each food on food detail screen
• Real-time calculation of total price in the cart screen
• Add desired food to the favorite screen
• Select quantity for each item on detail screen
• Filter foods by category
• State management with GetX | Cubit | Bloc | Provider
```

  <br/>

## Dependencies
|       Name      |    Cubit  <br/> version      |       Bloc <br/> version       |      GetX <br/> version     |    provider <br/> version   |
| :-------------: | :--------------------------: | :----------------------------: |  :------------------------: |  :------------------------: | 
| [flutter_bloc](https://pub.dev/packages/flutter_bloc)  |  ✔️  |  ✔️  |    ✖️    | ✖️    |
| [GetX](https://pub.dev/packages/get)  | ✖️  |  ✖️  | ✔️    |✖️    |
| [provider](https://pub.dev/packages/provider)  | ✖️  |  ✖️  | ✖️    | ✔️    | 
| [flutter_hooks](https://pub.dev/packages/flutter_hooks)  | ✔️  | ✔️  | ✖️ |✔️    | 
| [equatable](https://pub.dev/packages/equatable)  | ✔️  | ✔️  | ✖️ |✔️    | 
| [font_awesome_flutter](https://pub.dev/packages/font_awesome_flutter)  | ✔️  | ✔️ | ✔️ |✔️    | 
| [badges](https://pub.dev/packages/badges)  | ✔️  | ✔️ |✔️ |✔️    | 
| [animations](https://pub.dev/packages/animations)  | ✔️  | ✔️ |✔️ |✔️    | 
| [simple_animations](https://pub.dev/packages/simple_animations)  | ✔️  | ✔️ |✔️ |✔️    | 

  <br/>


## Directory Structure (GetX version)
```
📂lib
 │───main.dart  
 │───📂core  
 |   │──app_asset.dart
 |   │──app_color.dart
 |   │──app_data.dart
 |   │──app_icon.dart
 |   │──app_style.dart
 |   │──app_theme.dart
 |   └──app_extension.dart
 └───📂src
     │────📂model
     │    │──bottom_navigation_item.dart
     |    │──food.dart
     |    └──food_category.dart
     └────📂view
     |    │───📂screen
     |    |   |──cart_screen.dart
     |    |   |──favorite_screen.dart
     |    |   |──food_detail_screen.dart
     |    |   |──food_list_screen.dart
     |    |   |──home_screen.dart
     |    |   └──profile_screen.dart
     |    │───📂widget
     │    |   |──counter_button.dart
     │    |   |──custom_page_route.dart
     │    |   |──empty_widget.dart
     │    |   |──fade_animation.dart
     │    |   |──food_list_view.dart
     │    |   |──page_transition.dart
     |    |   └──scale_animation.dart
     └────📂controller
          └──food_controller.dart
```



## Directory Structure (Provider version)

```
📂lib
 │───main.dart  
 │───📂core  
 │   │──app_asset.dart
 │   │──app_color.dart
 │   │──app_data.dart
 │   │──app_icon.dart
 │   │──app_style.dart
 │   │──app_theme.dart
 │   └──app_extension.dart
 └───📂src
     │────📂data
     │    │───📂model
     │    │   |──bottom_navigation_item.dart
     │    │   |──food.dart
     │    │   └──food_category.dart
     │    │───📂repository
     │    │   └──repository.dart
     └────📂presentation
     │    │───📂screen
     │    │   |──cart_screen.dart
     │    │   |──favorite_screen.dart
     │    │   |──food_detail_screen.dart
     │    │   |──food_list_screen.dart
     │    │   |──home_screen.dart
     │    │   └──profile_screen.dart
     │    │───📂widget
     │    │   |──counter_button.dart
     │    │   |──custom_page_route.dart
     │    │   |──empty_widget.dart
     │    │   └──food_list_view.dart
     │    │───📂animation
     │    │   |──fade_animation.dart
     │    │   |──page_transition.dart
     │    │   └──scale_animation.dart
     └────📂business_logic
          └───📂provider
              │───📂food
              │   |──food_provider.dart
              │   └──food_state.dart
              └───📂category
              │    |──category_provider.dart
              │    └──category_state.dart
              └───📂theme
                   |──theme_provider.dart
                   └──theme_state.dart
```


## Directory Structure (Bloc version)

```
📂lib
 │───main.dart  
 │───📂core  
 │   │──app_asset.dart
 │   │──app_color.dart
 │   │──app_data.dart
 │   │──app_icon.dart
 │   │──app_style.dart
 │   │──app_theme.dart
 │   └──app_extension.dart
 └───📂src
     │────📂data
     │    │───📂model
     │    │   |──bottom_navigation_item.dart
     │    │   |──food.dart
     │    │   └──food_category.dart
     │    │───📂repository
     │    │   └──repository.dart
     └────📂presentation
     │    │───📂screen
     │    │   |──cart_screen.dart
     │    │   |──favorite_screen.dart
     │    │   |──food_detail_screen.dart
     │    │   |──food_list_screen.dart
     │    │   |──home_screen.dart
     │    │   └──profile_screen.dart
     │    │───📂widget
     │    │   |──counter_button.dart
     │    │   |──custom_page_route.dart
     │    │   |──empty_widget.dart
     │    │   └──food_list_view.dart
     │    │───📂animation
     │    │   |──fade_animation.dart
     │    │   |──page_transition.dart
     │    │   └──scale_animation.dart
     └────📂business_logic
          └───📂bloc
              │───📂food
              │   |──food_bloc.dart
              │   └──food_state.dart
              │   └──food_event.dart
              └───📂category
              │    |──category_bloc.dart
              │    └──category_state.dart
              │    └──category_event.dart
              └───📂theme
                   |──theme_bloc.dart
                   └──theme_state.dart
                   └──theme_event.dart
```


## Directory Structure (Cubit version)
```
📂lib
 │───main.dart  
 │───📂core  
 │   │──app_asset.dart
 │   │──app_color.dart
 │   │──app_data.dart
 │   │──app_icon.dart
 │   │──app_style.dart
 │   │──app_theme.dart
 │   └──app_extension.dart
 └───📂src
     │────📂data
     │    │───📂model
     │    │   |──bottom_navigation_item.dart
     │    │   |──food.dart
     │    │   └──food_category.dart
     │    │───📂repository
     │    │   └──repository.dart
     └────📂presentation
     │    │───📂screen
     │    │   |──cart_screen.dart
     │    │   |──favorite_screen.dart
     │    │   |──food_detail_screen.dart
     │    │   |──food_list_screen.dart
     │    │   |──home_screen.dart
     │    │   └──profile_screen.dart
     │    │───📂widget
     │    │   |──counter_button.dart
     │    │   |──custom_page_route.dart
     │    │   |──empty_widget.dart
     │    │   └──food_list_view.dart
     │    │───📂animation
     │    │   |──fade_animation.dart
     │    │   |──page_transition.dart
     │    │   └──scale_animation.dart
     └────📂business_logic
          └───📂cubits
              │───📂food
              │   |──food_cubit.dart
              │   └──food_state.dart
              └───📂category
              │    |──category_cubit.dart
              │    └──category_state.dart
              └───📂theme
                   |──theme_cubit.dart
                   └──theme_state.dart
```

<br>

## Created & Maintained By

[Dennis Nzioki](https://github.com/DNXEMPIRE-1) 

<br>


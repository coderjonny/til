When you have CONSTANTS in ruby classes you can reference them by using ```::```

```ruby
class School < ActiveRecord::Base
  DEFAULT_RANKS =
    [
      {"name"=>"Platinum", "color"=>"#dcdef6", "percent"=>97},
      {"name"=>"Diamond", "color"=>"#edfaf9", "percent"=>95},
      {"name"=>"Gold", "color"=>"#ede4aa", "percent"=>90},
      {"name"=>"Silver", "color"=>"#d6d6d6", "percent"=>85},
      {"name"=>"Bronze", "color"=>"#c48716", "percent"=>75}
    ]
end

School::DEFAULT_RANKS # get constant
```

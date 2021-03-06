# NumberToZhCn

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'number_to_zh_cn'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install number_to_zh_cn

## Usage

数字转成中文大写金额

number_to_capital_zh(10001.00)               # => '壹万元整',
number_to_capital_zh(100000.10)              # => '壹拾万元壹角整',
number_to_capital_zh(0.1)                    # => '壹角整',
number_to_capital_zh(1.11)                   # => '壹元壹角壹分',
number_to_capital_zh(1.01)                   # => '壹元零壹分',
number_to_capital_zh(0.01)                   # => '壹分',
number_to_capital_zh(1)                      # => '壹元整',
number_to_capital_zh(10)                     # => '壹拾元整',
number_to_capital_zh(100010.10)              # => '壹拾万零壹拾元壹角整',
number_to_capital_zh(100000000)              # => '壹亿元整',
number_to_capital_zh(1029.59)                # => '壹仟零贰拾玖元伍角玖分',
number_to_capital_zh(1029.58)                # => '壹仟零贰拾玖元伍角捌分',
number_to_capital_zh(1029.6)                 # => '壹仟零贰拾玖元陆角整',
number_to_capital_zh(1029)                   # => '壹仟零贰拾玖元整',

number_to_capital_zh(0)                      # => '零',
number_to_capital_zh(0.0)                    # => '零',
number_to_capital_zh(0.00)                   # => '零',
number_to_capital_zh(-0)                     # => '零',
number_to_capital_zh(-0.0)                   # => '零',
number_to_capital_zh(-0.00)                  # => '零',

number_to_capital_zh(-360.0)                 # => '负叁佰陆拾元整',
number_to_capital_zh(-10000.00)              # => '负壹万元整',
number_to_capital_zh(-100000.10)             # => '负壹拾万元壹角整',
number_to_capital_zh(-0.1)                   # => '负壹角整',
number_to_capital_zh(-1.11)                  # => '负壹元壹角壹分',
number_to_capital_zh(-1.01)                  # => '负壹元零壹分',
number_to_capital_zh(-0.01)                  # => '负壹分',
number_to_capital_zh(-1)                     # => '负壹元整',
number_to_capital_zh(-10)                    # => '负壹拾元整',
number_to_capital_zh(-100010.10)             # => '负壹拾万零壹拾元壹角整',
number_to_capital_zh(-100000000)             # => '负壹亿元整',
number_to_capital_zh(-1029.015)              # => '负壹仟零贰拾玖元零贰分',
number_to_capital_zh(-1029.59)               # => '负壹仟零贰拾玖元伍角玖分',
number_to_capital_zh(-1029.58)               # => '负壹仟零贰拾玖元伍角捌分',
number_to_capital_zh(-1029.6)                # => '负壹仟零贰拾玖元陆角整',
number_to_capital_zh(-1029)                  # => '负壹仟零贰拾玖元整',
number_to_capital_zh(-1029.015)              # => '负壹仟零贰拾玖元零贰分',


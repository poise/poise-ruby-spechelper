# PoiseRuby::SpecHelper

[![Build Status](https://img.shields.io/travis/poise/poise-ruby-spechelper.svg)](https://travis-ci.org/poise/poise-ruby-spechelper)
[![Gem Version](https://img.shields.io/gem/v/poise-ruby-spechelper.svg)](https://rubygems.org/gems/poise-ruby-spechelper)
[![Gemnasium](https://img.shields.io/gemnasium/poise/poise-ruby-spechelper.svg)](https://gemnasium.com/poise/poise-ruby-spechelper)
[![License](https://img.shields.io/badge/license-Apache_2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

This gem exists only to help with integration tests of [poise-ruby](https://github.com/poise/poise-ruby)
providers. It provides an RSpec shared example called `'a ruby_runtime_test'`
which verifies the correctness of `ruby_runtime_test` resource.

You can use this shared example by adding `gem 'poise-ruby-spechelper'` to
the Gemfile in your `serverspec/` folder. Then call it in your RSpec like:

```ruby
describe 'dummy provider' do
  it_should_behave_like 'a ruby_runtime_test', 'name'
end
```

## Sponsors

Development sponsored by [Bloomberg](http://www.bloomberg.com/company/technology/).

The Poise test server infrastructure is sponsored by [Rackspace](https://rackspace.com/).

## License

Copyright 2015, Noah Kantrowitz

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

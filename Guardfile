# A sample Guardfile
# More info at https://github.com/guard/guard#readme

notification :notifu, :time => 7, :nosound => true

guard 'phpunit', :cli => '--colors', :tests_path => 'app/tests' do
watch(%r{^.+Test.php$})
watch(%r{app/(.+)/(.+).php}) { |m| "tests/#{m[1]}/#{m[2]}Test.php" }
end

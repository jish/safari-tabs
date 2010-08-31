require 'erb'

desc 'Install scripts'
task :install => [:generate, :compile, :copy, :cleanup]

# desc 'Generate scripts'
task :generate do
  template = ERB.new(File.read('tab.applescript.erb'))

  (1..5).each do |i|
    File.open("tab#{i}.applescript", 'w') do |file|
      file.write(template.result(binding))
    end
  end
end

# desc 'Compile scripts'
task :compile do
  (1..5).each do |i|
    sh "osacompile -o tab#{i}.scpt tab#{i}.applescript"
  end
end

# desc 'Copy scripts to Safari scripts directory'
task :copy do
  sh 'mkdir -p ~/Library/Scripts/Applications/Safari/'
  sh 'cp *.scpt ~/Library/Scripts/Applications/Safari/'
end

# desc 'Cleanup generated files'
task :cleanup do
  sh 'rm *.applescript *.scpt'
end

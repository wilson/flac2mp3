# -*- ruby -*-

require 'rubygems'
require 'hoe'

Hoe.new('flac2mp3', '0.3.0') do |p|
  p.developer('Yossef Mendelssohn', 'ymendel@pobox.com')
  p.rubyforge_name = 'yomendel'
  p.extra_deps = [
    ['flacinfo-rb',  '>= 0.4'],
    ['ruby-mp3info', '>= 0.5.1'],
  ]
end

Rake.application.instance_eval { @tasks.delete("default") }
task :default do
  system "spec --options spec/spec.opts spec"
end

# vim: syntax=Ruby

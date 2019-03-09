require "rake/clean"

gutenberg_src_files = Rake::FileList.new("gutenberg/src/style/**/*.scss")

map = gutenberg_src_files.each_with_object({}) do |src, map|
  target = src
    .pathmap("%{gutenberg/src/style/_?,_sass/}p")
    .pathmap("%d/%{_?,_}f") # prepend underscore if missing

  CLOBBER << target

  map[target] = src
end

target_files = map.keys

task update: target_files

rule(%r{^_sass/.+} => ->(f) { map.fetch(f) }) do |t|
  mkdir_p t.name.pathmap("%d")
  cp t.source, t.name
end

task default: :update

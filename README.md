# httrobfuscate
[idea] Mirror website but obfuscating its content for performance tweaking/benchmarking.

Suppose you are working with web developers in a company with tight restrictions, maybe on a sensitive project, and the site is too slow. You know you can speed it up and break the 1000ms-to-glass barrier if you had root on a server. Well, you do have root on a server, but it's own VPS or RPi, and you cannot put company data on that server, and the company won't give you root on anything. Hamstrung!

Or suppose you are a freelancer looking to dazzle a prospective client whose site you could speed up, but you realize mirroring his site would be a bit presumptuous and perhaps illegal, and you don't want to ask the client first as it could undercut your sales pitch. How can you give him a side-by-side, while also presenting an appreciation for privacy? Would you take kindly to some tech guy you don't know mirroring your site, even locked down with a password?

Instead of just httracking the site and doing your web perf magic to it on your own server, why not httrack it, make a mirror out of it (or at least its statically-presented content), but with all the resources, including all text and all images and maybe video, totally obfuscated, so that your mirrored site looks the same to a webserver but foreign to a human eye, other than maybe the color scheme?

In other words, a mirror slash randomizer. A smart one that attempts to generate mock images that are not just the same dimensions as those it replaces but the same compression levels and maybe somehow random images of similar compression difficulty. Doing this manually takes too damn long. 

That's the gist, it's something that would have saved me a lot of time, I'd like to cobble something like this together, and here's my starting point. I don't know whether to fork httrack or fork some ipsum/lorem generator, this feels like a project that would incorporate a handful of existing open projects, not much that's original other than combining their functions. 

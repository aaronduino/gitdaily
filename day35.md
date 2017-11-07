# Day 35

It is possible to format the logs at will:

git log --pretty = format: '% Cred% h% Crescent% s% Cgreen (% cr)% Cblue <% an>'

With:

% C to change the color
% h for abbreviated SHA1
% s for the subject of commit
% cr for the relative date
% an for the author's name

More information about pretty format:

man git show

# sidebar-syllabus
document class for an information dense (and aesthetically pleasing) syllabus

Goals.

Create a document class that enables the following commands/document structure:

```latex
%%% Commands within the document %%%

%-----------------------------------
%% Print a sidebar:
%-----------------------------------

\sidebar[<color>,<image>]{
	<content>
}

%-----------------------------------
%% Sidebar content 
%-----------------------------------

\sidecontent[<header>]{<content>} % makes a textblock with this info

\coursedetails{
	\coursetext
	\coursetimelocation
	\courseetc % for notes like, ``no calculators'' or ``need WebAssign''
}

\profdetails{ % possibly multiple profs, so should be repeatable
	\profname
	\profoffice
	\profofficehours
	\profemail
	\profwebsite
}

\gradepie{<name>/<percentage>,...} % pie chart of grade weights

\gradetable{<A+>,<A>,<A->,<B+>,<B>,<B->,<C+>,<C>,<C->,<D+>,<D>,<D->}
	% table of grade minimum thresholds

\gradesbgtable{
	% not sure how to configure this yet?
}

\campusresources{
	% a nice list environment?
	\resource{<header>,<description>,<contact>} % formats resources
	\subresource{<header>,<description>,<contact>} % formats a list within a resource (eg DOS)
}

%-----------------------------------
%% Regular content
%-----------------------------------

\bodyquote[<header>]{<content>}
\bodysection[<header>]{<content>}
```

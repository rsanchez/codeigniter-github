CodeIgniter-GitHub
==================

Author
------

Philip Sturgeon - <email@philsturgeon.co.uk>

Description
-----------

CodeIgniter-GitHub is a CodeIgniter library which is essentially a wrapper for the GitHub API.

Usage
-----

Return an object for the given user, or returns false if the user does not exist

	$this->github_lib->user_info('bobbyjoe'); 
	
Return a list of commits for a project by a user. 

	$this->github_lib->user_timeline('philsturgeon', 'codeigniter-github');
	$this->github_lib->user_timeline('philsturgeon', 'codeigniter-github', 'branchname');
	
Return a list of repositories matching a search term. Optional 3rd parameter specifies programming language

	$this->github_lib->search('codeigniter');
	$this->github_lib->search('codeigniter', 'php');
	
Return a list of the repository info

	$this->github_lib->repo_info('philsturgeon', 'codeigniter-github');
	
Return a list of the repository's references

	$this->github_lib->repo_refs('philsturgeon', 'codeigniter-github', 'tags');
	$this->github_lib->repo_refs('philsturgeon', 'codeigniter-github', 'branches');
	
Return a list of issues for a project

	$this->github_lib->project_issues('philsturgeon', 'codeigniter-github', 'open');
	$this->github_lib->project_issues('philsturgeon', 'codeigniter-github', 'closed');

Extra
-----

If you'd like to request changes, report bug fixes, or contact
the developer of this library, email <email@philsturgeon.co.uk>
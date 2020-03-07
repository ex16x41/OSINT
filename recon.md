# targeted recon using dorks


# directory listing test
| Type | Desc |
|:---:|:---:|
| site:target.com intext:dir + "last modified" -pdf | - |
| site:target.com intitle:index.of | - |


# Configuration files 
| Type | Desc |
|:---:|:---:|
| site:target.com ext:xml OR ext:conf OR ext:cnf OR ext:reg OR ext:inf OR ext:rdp OR ext:cfg OR ext:txt OR ext:ora OR ext:ini | - |

# Database files 
| Type | Desc |
|:---:|:---:|
| site:target.com ext:sql OR ext:dbf OR ext:mdb | - |

# Log and Backup files 
| Type | Desc |
|:---:|:---:|
| site:target.com ext:bkf OR ext:bkp OR ext:bak OR ext:old OR ext:backup OR ext:log  | - |

# Login Portals 
| Type | Desc |
|:---:|:---:|
| site:target.com inurl:login  | - |

# SQL Errors
| Type | Desc |
|:---:|:---:|
| site:target.com intext:"sql syntax near" OR intext:"syntax error has occurred" OR intext:"incorrect syntax near" OR intext:"unexpected end of SQL command" OR intext:"Warning: mysql_connect()" OR intext:"Warning: mysql_query()" OR intext:"Warning: pg_connect()"  | - |

# Public Documents 
| Type | Desc |
|:---:|:---:|
| site:target.com ext:doc OR ext:docx OR ext:odt OR ext:pdf OR ext:rtf OR ext:sxw OR ext:psw OR ext:ppt OR ext:pptx OR ext:pps OR ext:csv  | - |

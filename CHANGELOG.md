## 0.9 (2017-06-20)

- New: Add support for non-image media types (requires libmagic)
- New: Allow lazy loading of objects
- New: Add WorkflowVersion class and Workflow.versions property
- Fix: Don't submit empty JSON by default for GET requests
- Fix: Adding location paths in Python 2
- Fix: Return a list of linked objects instead of a map in Python 3
- Use SetMemberSubject for SubjectSet.subjects lookup to improve speed
- Set default endpoint to www.zooniverse.org
- Raise TypeError if positional batchable argument is missing
- Convert Collection.subjects and SubjectSet.subjects to properties

## 0.8 (2017-05-11)

- New: Python 3 compatibility
- Fix: Fix passing sets to batchable methods
- Fix: `AttributeError` in `Workflow.add_subject_sets()`

## 0.7 (2017-03-22)

- New: Add Collection
- New: Allow editing of workflows
- New: Add method to get User's avatar
- New: Add support for iterating over numpy arrays
- New: Add per-Workflow exports
- Fix: setting endpoint in environment variable
- Fix: Stop iterating if there are no objects in the current page

## 0.6 (2017-01-11)

- New: Add Project.collaborators() and ProjectRole
- New: Add admin option
- Fix: Raise PanoptesAPIException instead of StopIteration
- Fix: Make ResultPaginator handle None responses
- Fix: Raise PanoptesAPIException instead of StopIteration in PanoptesObject.where()

## 0.5 (2016-11-21)

- New: Send SubjectSet.remove() requests in batches
- Fix: Raise PanoptesAPIException instead of StopIteration in Project.find()
- Fix: Don't read the image file on every upload attempt

## 0.4.1 (2016-09-21)

- Fix: Bearer token checking only occurs when necessary

## 0.4 (2016-09-02)

- New: Support for all data exports
- New: Project owners can update `ProjectPreference` settings
- New: Removed `subject_sets` method and `SetMemberSubject` (now in links)
- New: Add set to iterable types
- Fix: Only save links if it's been modified
- Fix: Specify minimum requests version

## 0.3 (2016-08-04)

- New: Add User model
- New: Add option for env vars for auth
- New: Add scope kwarg to Classification.where()
- New: Add SetMemberSubject class
- New: Submit subject links in batches in SubjectSet.add()
- New: oauth for client apps
- Fix: Skip trying to read export state if description was empty
- Fix: Don't rely on the response having a Content-Length header

## 0.2 (2016-07-21)

- New: Automatically retry failed image uploads
- New: Project classifications export
- New: Subject retirement in Workflow
- New: Add client ID for panoptes-staging.zooniverse.org
- New: Add ProjectPreferences
- New: Add Classification
- New: Removing subject set links
- Fix: IOError: Too many open files (in subject.py, line 64) #6

## 0.1 (2016-06-16)

- Initial release!
- Allows creating and modifying projects, subjects, subject sets

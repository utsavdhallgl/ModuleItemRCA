
# Module Items Performance Issue RCA

This documentation provides :
 - API calls happening in the content consumption page and their response data.
 - Meta Data required in the accordions in Content Navigator.
 - All the data (props) required for module items to work.

# API calls

### Module Item Sequence
- Example Endpoint: `https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/module_item_sequence?asset_id=36160&asset_type=ModuleItem&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response: ```{
    "items": [
        {
            "current": {
                "id": 36160,
                "title": "PGPBDA.C.Sep'17 - Meet Your Faculty",
                "position": 0,
                "indent": 0,
                "type": "File",
                "module_id": 7044,
                "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/36160",
                "content_id": 81085,
                "content_type": "application/pdf",
                "size": 372157,
                "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/81085",
                "last_published_at": null
            },
            "prev": null,
            "next": {
                "id": 35800,
                "title": "PGPBDA.C.Sep'17 - Schedule \u0026 Curriculum - Big Data Analytics",
                "position": 2,
                "indent": 0,
                "type": "File",
                "module_id": 7044,
                "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35800",
                "content_id": 79473,
                "content_type": "application/pdf",
                "size": 134581,
                "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/79473",
                "last_published_at": null
            }
        }
    ],
    "modules": [
        {
            "id": 7044,
            "name": "Program Overview",
            "position": 1,
            "unlock_at": null,
            "require_sequential_progress": false,
            "publish_final_grade": false,
            "prerequisite_module_ids": [],
            "completion_requirements": [],
            "items_count": 12,
            "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/7044/items"
        }
    ]
}```

### Module Item Data 
- Example Endpoint: `https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules?include[]=content_details&use_new_flow=true&student_id=6991&page=1&per_page=50&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response Data:`[
    {
        "id": 7044,
        "name": "Program Overview",
        "position": 1,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2017-09-18T16:01:17Z",
        "items_count": 12,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/7044/items"
    },
    {
        "id": 7045,
        "name": "Connect with Us",
        "position": 2,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2017-09-18T16:01:17Z",
        "items_count": 5,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/7045/items"
    },
    {
        "id": 7046,
        "name": "Practice Test/Assignment",
        "position": 3,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2017-09-18T16:00:09Z",
        "items_count": 2,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/7046/items"
    },
    {
        "id": 7415,
        "name": "Big Data Cloud Lab",
        "position": 5,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2017-10-08T11:18:42Z",
        "items_count": 3,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/7415/items"
    },
    {
        "id": 8571,
        "name": "Session with Dr. Narayana",
        "position": 6,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2018-01-03T12:31:23Z",
        "items_count": 1,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/8571/items"
    },
    {
        "id": 8971,
        "name": "Additional Statistical Learning Doubt Clearing Session by Prof. Gurumoorthy",
        "position": 7,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2018-01-22T06:15:15Z",
        "items_count": 9,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/8971/items"
    },
    {
        "id": 8994,
        "name": "Online Conference of Machine Learning on AWS",
        "position": 8,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2018-01-22T06:15:15Z",
        "items_count": 2,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/8994/items"
    },
    {
        "id": 10255,
        "name": "Instructions to Install Python Packages in Cloud Lab",
        "position": 10,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2018-03-17T05:51:38Z",
        "items_count": 1,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/10255/items"
    },
    {
        "id": 10917,
        "name": "Articles",
        "position": 11,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2018-06-01T14:53:42Z",
        "items_count": 1,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/10917/items"
    },
    {
        "id": 12240,
        "name": "Conferences",
        "position": 12,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2018-06-01T14:53:42Z",
        "items_count": 2,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/12240/items"
    }
]`
### Announcement Count
- Example Endpoint: `https://stelevate.iac-mygreatlearning.net/api/v1/announcements/count?course_ids[]=1679&course_ids[]=247&course_ids[]=1607&course_ids[]=1622&course_ids[]=2442&course_ids[]=1617&course_ids[]=2412&course_ids[]=1618&course_ids[]=1620&course_ids[]=1621&course_ids[]=1616&course_ids[]=1811&course_ids[]=1754&course_ids[]=1612&course_ids[]=1615&course_ids[]=1609&course_ids[]=1611&course_ids[]=1610&course_ids[]=1608&group_ids[]=9232&group_ids[]=10421&group_ids[]=10544&group_ids[]=10415&group_ids[]=10686&group_ids[]=9631&group_ids[]=9913&group_ids[]=8510&group_ids[]=10272&group_ids[]=9034&user_id=6991&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response: `{
    "course": {
        "count": 391,
        "grouped_count": {
            "247": 154,
            "1607": 71,
            "1608": 12,
            "1609": 7,
            "1610": 4,
            "1611": 8,
            "1612": 11,
            "1615": 11,
            "1616": 9,
            "1617": 10,
            "1618": 11,
            "1620": 16,
            "1621": 15,
            "1622": 14,
            "1754": 9,
            "1811": 10,
            "2412": 12,
            "2442": 7
        }
    },
    "group": {
        "count": 2,
        "grouped_count": {
            "9913": 2
        }
    },
    "general": {
        "count": 0
    }
}`
### Course Progress:
- Example Endpoint: `https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/progress?user_id=6991&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response: `{
    "percentage": 26,
    "remainingSeconds": 0,
    "module_progress": {
        "7044": {
            "percentage": 75,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 1,
            "total_assessments": 3,
            "completed_resources": 8,
            "total_resources": 9,
            "new_item_count": 0,
            "completed": false
        },
        "7045": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 5,
            "new_item_count": 0,
            "completed": false
        },
        "7046": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 2,
            "completed_resources": 0,
            "total_resources": 0,
            "new_item_count": 0,
            "completed": false
        },
        "7415": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 3,
            "new_item_count": 0,
            "completed": false
        },
        "8571": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 1,
            "new_item_count": 0,
            "completed": false
        },
        "8971": {
            "percentage": 11,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 2,
            "completed_resources": 1,
            "total_resources": 7,
            "new_item_count": 0,
            "completed": false
        },
        "8994": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 2,
            "new_item_count": 0,
            "completed": false
        },
        "10255": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 1,
            "new_item_count": 0,
            "completed": false
        },
        "10917": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 1,
            "new_item_count": 0,
            "completed": false
        },
        "12240": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 2,
            "new_item_count": 0,
            "completed": false
        }
    },
    "completed_videos": 0,
    "total_videos": 0,
    "completed_assessments": 1,
    "total_assessments": 7,
    "completed_resources": 9,
    "total_resources": 31,
    "marks": 10,
    "total_marks": 10,
    "grade": "On Track",
    "is_gpa_grading_scheme": false
}`

### Current Module Item Data:
- Example Endpoint: `  
https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/modules/7044/items/36160?include[]=content_details&student_id=6991&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response Data: `{
    "item": {
        "id": 36160,
        "title": "PGPBDA.C.Sep'17 - Meet Your Faculty",
        "position": 0,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/36160",
        "content_id": 81085,
        "content_type": "application/pdf",
        "size": 372157,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/81085",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Meet Your Faculty-1.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/81085"
    },
    "module": {
        "id": 7044,
        "name": "Program Overview",
        "position": 1,
        "unlock_at": null,
        "require_sequential_progress": false,
        "publish_final_grade": false,
        "prerequisite_module_ids": [],
        "completion_requirements": [],
        "state": "completed",
        "completed_at": "2017-09-18T16:01:17Z",
        "items_count": 12,
        "items_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/modules/7044/items"
    }
}`
### New Course Items
- Example Endpoint: `https://stelevate.iac-mygreatlearning.net/api/v1/new_course_items/users/6991?pb_id=70&skip_staging_auth=1&source=web_app`
- Example Response Data: `[]`
### Asset Access:
- Example Endpoint: `https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/asset_access?user_id=6991&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response Data: `[
    {
        "asset_code": "wiki_page_20830",
        "asset_category": "wiki",
        "display_name": "PGPBDA.C.Sep'17 - Know Your Classmates"
    },
    {
        "asset_code": "discussion_topic_14497",
        "asset_category": "topics",
        "display_name": "PGPBDA.C.Sep'17 - Introduce Yourself"
    },
    {
        "asset_code": "attachment_79476",
        "asset_category": "files",
        "display_name": "PGPBDA.C.Sep'17 - Program Evaluation Policy.pdf"
    },
    {
        "asset_code": "attachment_79479",
        "asset_category": "files",
        "display_name": "PGPBDA.C.Sep'17 - Acceptable Use Policy.pdf"
    },
    {
        "asset_code": "attachment_81085",
        "asset_category": "files",
        "display_name": "PGPBDA.C.Sep'17 - Meet Your Faculty-1.pdf"
    },
    {
        "asset_code": "attachment_79475",
        "asset_category": "files",
        "display_name": "PGPBDA.C.Sep'17 - Students HandBook.pdf"
    },
    {
        "asset_code": "wiki_page_22991",
        "asset_category": "wiki",
        "display_name": "Residency Plan"
    },
    {
        "asset_code": "quizzes:quiz_3284",
        "asset_category": "quizzes",
        "display_name": "Statistics Doubt Clearing Session Survey"
    },
    {
        "asset_code": "discussion_topic_19332",
        "asset_category": "topics",
        "display_name": "Topics to be addressed in Additional Statistical Learning Doubt Clearing Session by Prof. Gurumoorthy"
    },
    {
        "asset_code": "attachment_99969",
        "asset_category": "files",
        "display_name": "PGPBDA.C.Sep 17- Program Curriculum Details.pdf"
    },
    {
        "asset_code": "attachment_79473",
        "asset_category": "files",
        "display_name": "PGPBDA.C.Sep'17 - Schedule & Curriculum - Big Data Analytics.pdf"
    },
    {
        "asset_code": "attachment_126105",
        "asset_category": "files",
        "display_name": "NCMLAI 2018 - BROCHURE.pdf"
    },
    {
        "asset_code": "quizzes:quiz_3840",
        "asset_category": "quizzes",
        "display_name": "Change in Residency date in May 2018 Survey"
    },
    {
        "asset_code": "quizzes:quiz_2675",
        "asset_category": "quizzes",
        "display_name": "Try Me"
    },
    {
        "asset_code": "quizzes:quiz_3309",
        "asset_category": "quizzes",
        "display_name": "Feedback for Additional Statistical Learning Doubt Clearing Session by Prof. Gurumoorthy - 28th January 2018"
    },
    {
        "asset_code": "attachment_112183",
        "asset_category": "files",
        "display_name": "hypothesis testing and chi square test.pdf"
    },
    {
        "asset_code": "assignment_4745",
        "asset_category": "assignments",
        "display_name": "My Assignment"
    }
]`
### Items in the current Module:
- Endpoint: `https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/modules/7044/items?include[]=content_details&student_id=6991&page=1&per_page=50&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response: `[
    {
        "id": 36160,
        "title": "PGPBDA.C.Sep'17 - Meet Your Faculty",
        "position": 0,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/36160",
        "content_id": 81085,
        "content_type": "application/pdf",
        "size": 372157,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/81085",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Meet Your Faculty-1.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/81085"
    },
    {
        "id": 35800,
        "title": "PGPBDA.C.Sep'17 - Schedule & Curriculum - Big Data Analytics",
        "position": 2,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35800",
        "content_id": 79473,
        "content_type": "application/pdf",
        "size": 134581,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/79473",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Schedule & Curriculum - Big Data Analytics.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/79473"
    },
    {
        "id": 35748,
        "title": "PGPBDA.C.Sep'17 - Know Your Classmates",
        "position": 3,
        "indent": 0,
        "type": "Page",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35748",
        "page_url": "pgpbda-dot-c-sep17-know-your-classmates",
        "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/pages/pgpbda-dot-c-sep17-know-your-classmates",
        "last_published_at": null,
        "content_details": {
            "locked_for_user": false
        },
        "contentMeta": {
            "module_item_id": 35748,
            "content_id": 20830,
            "content_type": "WikiPage"
        },
        "isNew": false,
        "isViewed": true
    },
    {
        "id": 35749,
        "title": "PGPBDA.C.Sep'17 - Introduce Yourself",
        "position": 4,
        "indent": 0,
        "type": "Discussion",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35749",
        "content_id": 14497,
        "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/discussion_topics/14497",
        "last_published_at": null,
        "content_details": {
            "locked_for_user": false
        },
        "contentMeta": {
            "content_id": 14497,
            "muted": null,
            "submitted_at": null,
            "grade": null,
            "submission_state": null,
            "content_type": "DiscussionTopic",
            "feedback_rating": null
        },
        "isNew": false,
        "isViewed": true
    },
    {
        "id": 35801,
        "title": "PGPBDA.C.Sep'17 - Students HandBook",
        "position": 5,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35801",
        "content_id": 79475,
        "content_type": "application/pdf",
        "size": 258675,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/79475",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Students HandBook.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/79475"
    },
    {
        "id": 35802,
        "title": "PGPBDA.C.Sep'17 - Program Evaluation Policy",
        "position": 6,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35802",
        "content_id": 79476,
        "content_type": "application/pdf",
        "size": 213006,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/79476",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Program Evaluation Policy.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/79476"
    },
    {
        "id": 35804,
        "title": "PGPBDA.C.Sep'17 - Acceptable Use Policy",
        "position": 8,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35804",
        "content_id": 79479,
        "content_type": "application/pdf",
        "size": 207382,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/79479",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Acceptable Use Policy.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/79479"
    },
    {
        "id": 35805,
        "title": "PGPBDA.C.Sep'17 - Technical Requirements (HW & SW)",
        "position": 9,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/35805",
        "content_id": 79480,
        "content_type": "application/pdf",
        "size": 79582,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/79480",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep'17 - Technical Requirements (HW & SW).pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": false,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/79480"
    },
    {
        "id": 42743,
        "title": "PGPBDA.C.Sep 17- Program Curriculum Details.pdf",
        "position": 11,
        "indent": 0,
        "type": "File",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/42743",
        "content_id": 99969,
        "content_type": "application/pdf",
        "size": 678126,
        "url": "https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/files/99969",
        "last_published_at": null,
        "content_details": {
            "display_name": "PGPBDA.C.Sep 17- Program Curriculum Details.pdf",
            "locked_for_user": false
        },
        "isNew": false,
        "isViewed": true,
        "preview_url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/files/99969"
    },
    {
        "id": 42746,
        "title": "Residency Plan",
        "position": 12,
        "indent": 0,
        "type": "Page",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/42746",
        "page_url": "residency-plan",
        "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/pages/residency-plan",
        "last_published_at": null,
        "content_details": {
            "locked_for_user": false
        },
        "contentMeta": {
            "module_item_id": 42746,
            "content_id": 22991,
            "content_type": "WikiPage"
        },
        "isNew": false,
        "isViewed": true
    },
    {
        "id": 45066,
        "title": "Statistics Doubt Clearing Session Survey",
        "position": 13,
        "indent": 0,
        "type": "Quiz",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/45066",
        "content_id": 3284,
        "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/quizzes/3284",
        "last_published_at": null,
        "content_details": {
            "due_at": "2018-01-21T17:30:00Z",
            "lock_at": "2018-01-21T17:30:00Z",
            "locked_for_user": true,
            "lock_info": {
                "asset_string": "quizzes:quiz_3284",
                "lock_at": "2018-01-21T17:30:00Z",
                "can_view": true
            },
            "lock_explanation": "This quiz was locked Jan 21, 2018 at 11pm."
        },
        "contentMeta": {
            "content_id": 3284,
            "muted": null,
            "submitted_at": null,
            "grade": null,
            "submission_state": null,
            "content_type": "Quizzes::Quiz",
            "feedback_rating": null,
            "quiz_type": "survey"
        },
        "isNew": false,
        "isViewed": true
    },
    {
        "id": 52020,
        "title": "Change in Residency date in May 2018 Survey",
        "position": 14,
        "indent": 0,
        "type": "Quiz",
        "module_id": 7044,
        "html_url": "https://mgolympus.iac-mygreatlearning.net/courses/1607/modules/items/52020",
        "content_id": 3840,
        "url": "https://mgolympus.iac-mygreatlearning.net/api/v1/courses/1607/quizzes/3840",
        "last_published_at": null,
        "content_details": {
            "due_at": "2018-03-26T17:30:00Z",
            "unlock_at": "2018-03-24T06:30:00Z",
            "lock_at": "2018-03-26T17:30:00Z",
            "locked_for_user": true,
            "lock_info": {
                "asset_string": "quizzes:quiz_3840",
                "lock_at": "2018-03-26T17:30:00Z",
                "can_view": true
            },
            "lock_explanation": "This quiz was locked Mar 26, 2018 at 11pm."
        },
        "contentMeta": {
            "content_id": 3840,
            "muted": null,
            "submitted_at": "2018-03-25T11:29:12.117Z",
            "grade": 1,
            "submission_state": "complete",
            "content_type": "Quizzes::Quiz",
            "feedback_rating": null,
            "quiz_type": "survey"
        },
        "isNew": false,
        "isViewed": true
    }
]`
### Course Progress:
- Endpoint : `https://stelevate.iac-mygreatlearning.net/api/v1/courses/1607/progress?user_id=6991&skip_staging_auth=1&pb_id=70&source=web_app`
- Example Response: `{
    "percentage": 26,
    "remainingSeconds": 0,
    "module_progress": {
        "7044": {
            "percentage": 75,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 1,
            "total_assessments": 3,
            "completed_resources": 8,
            "total_resources": 9,
            "new_item_count": 0,
            "completed": false
        },
        "7045": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 5,
            "new_item_count": 0,
            "completed": false
        },
        "7046": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 2,
            "completed_resources": 0,
            "total_resources": 0,
            "new_item_count": 0,
            "completed": false
        },
        "7415": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 3,
            "new_item_count": 0,
            "completed": false
        },
        "8571": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 1,
            "new_item_count": 0,
            "completed": false
        },
        "8971": {
            "percentage": 11,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 2,
            "completed_resources": 1,
            "total_resources": 7,
            "new_item_count": 0,
            "completed": false
        },
        "8994": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 2,
            "new_item_count": 0,
            "completed": false
        },
        "10255": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 1,
            "new_item_count": 0,
            "completed": false
        },
        "10917": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 1,
            "new_item_count": 0,
            "completed": false
        },
        "12240": {
            "percentage": 0,
            "completed_videos": 0,
            "total_videos": 0,
            "completed_assessments": 0,
            "total_assessments": 0,
            "completed_resources": 0,
            "total_resources": 2,
            "new_item_count": 0,
            "completed": false
        }
    },
    "completed_videos": 0,
    "total_videos": 0,
    "completed_assessments": 1,
    "total_assessments": 7,
    "completed_resources": 9,
    "total_resources": 31,
    "marks": 10,
    "total_marks": 10,
    "grade": "On Track",
    "is_gpa_grading_scheme": false
}`

# Meta Data in Accordions

- Assessments Count
- Resources

## Individual Items in Accordion

- Item Icon 
- Item Name
- Item Status (Locked, Complete, Pending)

# Props required for each module item

## Assignments

- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul
- **onViewed**: Callback Provided by Rahul
- **courseId**
- **moduleId**
- **assignmentId**
- **moduleItemId**

## Discussion Questions

- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul
- **onViewed**: Callback Provided by Rahul
- **courseId**
- **discussionTopicId**
- **moduleItemId**

## Quiz

- **courseId**
- **quizId**  
- **contentId**: Same as module Item Id
- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul
- **onViewed**: Callback Provided by Rahul
- **moduleItemId**
- **moduleId**

## Course External URL viewer

- **courseId**
- **moduleItemId**
- **moduleId**
- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul

## Course External Tool Viewer

- **courseId**
- **moduleItemId**
- **moduleId**
- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul

## Course File Viewer

- **courseId**
- **moduleItemId**
- **moduleId**
- **contentId**
- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul

## Course Video Viewer

- **courseId**
- **moduleItemId**
- **moduleId**
- **contentId**
- **resumeFrom**
- **fileKey**
- **onBackPress**
- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul

## Course Wiki Page Viewer

-  **courseId**
- **moduleItemId**
- **onLoaded**: Callback Provided by Rahul
- **onComplete**: Callback Provided by Rahul
- **pageUrl**

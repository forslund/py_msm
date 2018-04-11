## Py MSM

Mycroft Skill Manager, in python!

## install

    pip install py_msm

## Usage

    from py_msm import MycroftSkillsManager

    msm = MycroftSkillsManager()
    
    # msm = MycroftSkillsManager(skills_config={"directory":"some/test/path"})
    
    print msm.platform
    print msm.default_skills
    print msm.list_skills()
    print msm.url_info("https://github.com/JarbasAl/skill-stephen-hawking")
    print msm.name_info("date time")
    msm.update_skills()
    msm.remove_by_name("stephen hawking")
    msm.install_by_name("diagnostics")
    msm.install_defaults()

## TODO

- messagebus messages for mycroft-core interaction
- testing permissions issues in mark1/picroft
- standalone command line util
- mycroft skill with stats about skills repo and installed skills
- [create readme.md](https://rawgit.com/MycroftAI/mycroft-skills/master/meta_editor.html)
- parse readme.md
- skiller.sh functionality
- submit skill to skills repo
- documentation

## troubleshooting

got problem? most likely you forgot 

    workon mycroft
    
this needs mycroft core installed to run, which in a desktop implies virtual env installation


## Credits

JarbasAI
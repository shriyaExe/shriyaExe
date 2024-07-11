```python
class Developer:
    def __init__(self):
        self.skills = [
            "Python",
            "Django",
            "PostgreSQL",
            "AWS",
            "ReactJs",
            "Flutter"
        ]

    def __str__(self):
        bio = (
            "class Developer:\n"
            "    def __init__(self):\n"
            "        self.skills = [\n"
        )
        for skill in self.skills:
            bio += f"            '{skill}',\n"
        bio += (
            "        ]\n\n"
            "    def __str__(self):\n"
            "        bio = 'Developer Skillset:\\n'\n"
            "        for skill in self.skills:\n"
            "            bio += f'- {skill}\\n'\n"
            "        return bio"
        )
        return bio

    def display_skills(self):
        bio = "Developer Skillset:\n"
        for skill in self.skills:
            bio += f"- {skill}\n"
        return bio


developer = Developer()
print(developer)

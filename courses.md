---
layout: default
---

# Courses I've Taught

<table class="pure-table pure-table-bordered">
    <thead>
        <tr>
            <th>Term</th>
            <th>Course</th>
            <th>Role</th>
            <th>School</th>
        </tr>
    </thead>

    <tbody>
        {% for course in site.data.courses %}
            <tr>
                <td>{{ course.term }}</td>
                <td>
                    {% if course.url %}
                        <a href="{{ course.url }}">{{ course.name }}</a>
                    {% else %}
                        {{ course.name }}
                    {% endif %}
                </td>
                <td>{{ course.role }}</td>
                <td>{{ course.school }}</td>
            </tr>
        {% endfor %}
    </tbody>
</table>

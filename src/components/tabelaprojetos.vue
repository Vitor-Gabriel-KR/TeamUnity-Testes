    <!-- <template>
        <div>
        <md-table v-model="searched" md-sort="name" md-sort-order="asc" md-card md-fixed-header>
            <md-table-toolbar>
            <div class="md-toolbar-section-start">
                <h1 class="md-title">Users</h1>
            </div>
    
            <md-field md-clearable class="md-toolbar-section-end">
                <md-input placeholder="Search by name..." v-model="search" @input="searchOnTable" />
            </md-field>
            </md-table-toolbar>
    
            <md-table-empty-state
            md-label="No users found"
            :md-description="`No user found for this '${search}' query. Try a different search term or create a new user.`">
            <md-button class="md-primary md-raised" @click="newUser">Create New User</md-button>
            </md-table-empty-state>
    
            <md-table-row slot="md-table-row" slot-scope="{ item }">
            <md-table-cell md-label="ID" md-sort-by="id" md-numeric>{{ item.id }}</md-table-cell>
            <md-table-cell md-label="Name" md-sort-by="name">{{ item.name }}</md-table-cell>
            <md-table-cell md-label="Email" md-sort-by="email">{{ item.email }}</md-table-cell>
            <md-table-cell md-label="Gender" md-sort-by="gender">{{ item.gender }}</md-table-cell>
            <md-table-cell md-label="Job Title" md-sort-by="title">{{ item.title }}</md-table-cell>
            </md-table-row>
        </md-table>
        </div>
    </template>
    
    <script setup lang="ts">
    import { ref, Ref } from 'vue';
    
    interface User {
        id: number;
        name: string;
        email: string;
        gender: string;
        title: string;
    }
    
    const toLower = (text: string): string => {
        return text.toLowerCase();
    };
    
    const searchByName = (items: User[], term: string): User[] => {
        if (term) {
        return items.filter(item => toLower(item.name).includes(toLower(term)));
        }
        return items;
    };
    
    const search: Ref<string | null> = ref(null);
    const searched: Ref<User[]> = ref([]);
    const users: User[] = [
        {
        id: 1,
        name: "Shawna Dubbin",
        email: "sdubbin0@geocities.com",
        gender: "Male",
        title: "Assistant Media Planner"
        },
          {
            id: 2,
            name: "Odette Demageard",
            email: "odemageard1@spotify.com",
            gender: "Female",
            title: "Account Coordinator"
          },
          {
            id: 3,
            name: "Vera Taleworth",
            email: "vtaleworth2@google.ca",
            gender: "Male",
            title: "Community Outreach Specialist"
          },
          {
            id: 4,
            name: "Lonnie Izkovitz",
            email: "lizkovitz3@youtu.be",
            gender: "Female",
            title: "Operator"
          },
          {
            id: 5,
            name: "Thatcher Stave",
            email: "tstave4@reference.com",
            gender: "Male",
            title: "Software Test Engineer III"
          },
          {
            id: 6,
            name: "Karim Chipping",
            email: "kchipping5@scribd.com",
            gender: "Female",
            title: "Safety Technician II"
          },
          {
            id: 7,
            name: "Helge Holyard",
            email: "hholyard6@howstuffworks.com",
            gender: "Female",
            title: "Internal Auditor"
          },
          {
            id: 8,
            name: "Rod Titterton",
            email: "rtitterton7@nydailynews.com",
            gender: "Male",
            title: "Technical Writer"
          },
          {
            id: 9,
            name: "Gawen Applewhite",
            email: "gapplewhite8@reverbnation.com",
            gender: "Female",
            title: "GIS Technical Architect"
          },
          {
            id: 10,
            name: "Nero Mulgrew",
            email: "nmulgrew9@plala.or.jp",
            gender: "Female",
            title: "Staff Scientist"
          },
        ]
        const newUser = (): void => {
        window.alert('Noop');
        };

        const searchOnTable = (): void => {
        searched.value = searchByName(users, search.value || '');
        };

        searched.value = users;
        </script>

        <style scoped>
        </style> -->
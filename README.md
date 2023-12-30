# Museum Database Management System  
# Description of the problem
These days, we are witnessing a lack of visitors in museums, one of the reasons for which is the lack of a clear database that contains a list of museums and their fields. Visiting museums constantly enriches discussions, teamwork and sharing ideas among the participants, and the experience that visitors get from museums makes them comprehensive in understanding the various aspects of life. Therefore, exploring museums provides visitors with the willingness to participate enthusiastically in the process of acquiring information beyond  their realm of knowledge. To make this list easier for visitors or even tourists, we will create a database of museums to make this process easier and easier. We need this information the name of the museum, its type, in which gallery it will be displayed, and reservation information such as the number of people who will visit it, and the time and date.

# Scenario description
- Many visitors can visit the museum by making a reservation.
- The reservation is necessary for the visitors to enter the museum.
- Reservations of visitors including all the information such as: number of 
reservations, payment method, and total are kept in records.
- A single gallery may display many paintings.
- Painting owned by only one artist.
- Artist can have many Paintings.
- Each gallery has many staff works in it.
- A single staff could have many skills.
- Each gallery has name, id, address, and space.


# Entities
Gallery: contains the gallery id, name, address, and size this information is to identify 
each gallery.
Staff: has ids, names, phone, and emails to communicate with them and a single staff 
can have many skills 
Staff_skill: shows the skills of each employee.
Painting: is identified by a number has a size.
Artist: identified by id, has a name, email, phone, and each artist has a distinct type of 
art.
Reservation: has a number, payment method and the date of reservation.
Visitor: every visitor to the museum is identified uniquely by an id has a name, email, 
and phone number.

# Functional Dependency
 gallery_id#, ->gallery_name, gallery_address, length, width
staff_id# -> staff_name, date_of_birth, salary, staff phone, staff_emial
visitor_id# -> visitor_name, visitor_phone, visitor_email
staff_id#, skill# -> skill
res_no# -> payment_method, total
painting_number# -> height, width, artist_id#, artist_name, artist_phone, artist_email, type_of_art

import { workouts } from "./data.js"

const workoutsInfo = JSON.parse(workouts);

function renderWorkoutSchedule(workoutsInfo) {
    const scheduleBox = document.querySelector('.schedule-box');

    workoutsInfo.forEach(item => {
        scheduleBox.insertAdjacentHTML('beforeend', `
        <div class="schedule_item-box" id="${item.name_of_workout}">
			<div class="schedule_item">
            <p class="schedule_item-title">${item.name_of_workout}</p>
            <p class="schedule_item-time">${item.time_of_workout}</p>
			<p class="schedule_item-maxnumber">Максимальное количество участников: <span>${item.max_number_of_participants}</span></p>
            <p data-id=${item.id} class="schedule_item-currentnumber">Текущее количество записанных участников: <span>${item.current_number_of_participants}</span></p>
            <div class="button-box">
            <button class="button-submit" id="${item.id}">Записаться</button>
            <button class="button-reject" data-id="${item.name_of_workout}">Отменить запись</button>
            </div>
		</div>
        `)

    });
}
renderWorkoutSchedule(workoutsInfo);


const scheduleBox = document.querySelector('.schedule-box');


scheduleBox.addEventListener('click', function (e) {

    if (e.target.classList.contains('button-submit')) {
        workoutsInfo[e.target.id - 1].current_number_of_participants++;
        const currentNumberOfParticipants = document.querySelector(`[data-id="${e.target.id}"]`);
        const span = currentNumberOfParticipants.querySelector('span');
        span.textContent = workoutsInfo[e.target.id - 1].current_number_of_participants;
        const currentSubmitButton = document.getElementById(`${e.target.id}`);
        if (workoutsInfo[e.target.id - 1].current_number_of_participants == workoutsInfo[e.target.id - 1].max_number_of_participants) {

            currentSubmitButton.classList.add('disabled');
            currentSubmitButton.nextElementSibling.classList.remove('disabled');
        }
        else {
            currentSubmitButton.classList.remove('disabled');
        }


    }

    if (e.target.classList.contains('button-reject')) {
        let currentWorkoutsInfoItem = workoutsInfo.filter(item => item.name_of_workout === e.target.dataset.id);
        let index = Number(currentWorkoutsInfoItem[0].id) - 1;
        workoutsInfo[index].current_number_of_participants = workoutsInfo[index].current_number_of_participants - 1;
        const currentNumberOfParticipants = document.querySelector(`[data-id="${index + 1}"]`);
        const span = currentNumberOfParticipants.querySelector('span');
        span.textContent = workoutsInfo[index].current_number_of_participants;
        const currentRejectButton = document.querySelector(`[data-id="${e.target.dataset.id}"]`);

        if (workoutsInfo[index].current_number_of_participants <= 0) {
            currentRejectButton.classList.add('disabled');
        } else {
            currentRejectButton.classList.remove('disabled');

        }
    }
});
